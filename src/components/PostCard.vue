<template>
  <div class="postcard">
    <h1>{{ msg }}</h1>
   </div>
</template>

<script>
export default {
  name: 'PostCard',
  props: {
    msg: String   //do they both need msg prop? This and PostCardForm? Or just one?
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
