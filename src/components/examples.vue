
<template>
  <div class="hello">
    <h1>Using v-text{{msg}}</h1>
    <p>Using v-html: <span v-html="html"></span></p>
    <h2>My deepest, darkest question: {{existentialQuestion}}</h2>
    <input v-model="existentialQuestion"/>


</div>
</template>

<script>


export default {
  name: 'Examples',
  props: {
    msg: String, //msg
    html: String, //'This is a message for <a href="#">John Doe</a>, please update your email address.'
    // existentialQuestion: String
  },

  data() {
    return {
      existentialQuestion: ''
    };
  }
}



</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
