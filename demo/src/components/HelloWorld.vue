<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Hello World</h2>
    <p>innerState: {{innerState}}</p>
    <a-button @click="++innerState">change innerState</a-button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: ['msg'],
  data(){
    return {
      innerState: 1 
    }
  },

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
