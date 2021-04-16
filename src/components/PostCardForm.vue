<template>
  <div class="postcard-form">
    <h2>This is where the form will live</h2>
    <textarea class="postcard-text">Enter Your Text:</textarea>
  </div>
</template>

<!--  v-model="msg"  used in the textarea tag, but that broke it-->
<!-- <input :value="value" @input="$emit('input', $event.target.value)"> 
the above could be using input instead of textarea -->



<script>
export default {
  name: 'PostCardForm',
  props: {
    msg: {
      type: String,
      default: 'Enter message',
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
