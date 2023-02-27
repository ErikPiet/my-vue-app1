<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Welkom bij de eerste Vue-applicatie van {{ name }}.
    </p>
    <AppList />
  </div>
</template>

<script>
import AppList from  "@/components/AppList";
export default {
  name: 'HelloWorld',
  components: {AppList},
  props: {
    msg: String,
    name: String
  }  
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body {
  color: rgba(41,52,57,0);
}
h1 {
  margin: 40px 0 0;
  color: rgba(0,170,162,255);
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
