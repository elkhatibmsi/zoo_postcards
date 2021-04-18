<template>
  <div class="postcard-form">
    <h2>This is where the form will live</h2>
    <input class="postcard-text" :msg="msg" placeholder="Enter your message..." @input="$emit('placeholder', msg)">
  </div>
  <p class="message-output">
      Your message is: {{ msg }}
  </p>
</template>

<!--How to emit msg to PostCard? Does PostCardForm need it at all?-->

<script>
export default {
  name: 'PostCardForm',
  props: {
    msg: {
      type: String,
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
