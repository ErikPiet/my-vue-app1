<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Welkom bij de eerste Vue-applicatie van {{ name }}.
    </p>
    <CustomerList />
    <EigenComponent lstname="Piet" />
  </div>
</template>

<script>
import CustomerList from  "@/components/CustomerList";
import EigenComponent from  "@/components/EigenComponent";
export default {
  name: 'HelloWorld',
  components: {CustomerList, EigenComponent},
  props: {
    msg: String,
    name: String
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
