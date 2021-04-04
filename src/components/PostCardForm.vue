<template>
  <div class="postcard-form">
    <h2>This is where the form will live</h2>
    <textarea class="postcard-text" v-model="msg">Enter Your Text:</textarea>
  </div>
</template>

<script>
export default {
  name: 'PostCardForm',
  props: {
    msg: {
      type: 'text',
      value: 'Enter message',
      required: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>


<!--
Adapt this method:

onSubmit() {
          if (this.name === '' || this.review === '' || this.rating === null) {
              alert('Review is incomplete. Please fill out every field.')
              return
          }
          let productReview = {
              name: this.name,
              review: this.review,
              rating: this.rating
          }
          this.$emit('review-submitted', productReview)
          
          this.name = ''
          this.review = ''
          this.rating = null
      }
-->
