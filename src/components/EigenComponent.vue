<template>
    <div>
      <h2>Ons gezin {{ lstname }}</h2>
      <ul>
          <li>Erik</li>
          <li>Daan</li>
          <li>Dan</li>
          <li>Ian</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    name: 'EigenComponent',
    props: {   
        lstname: String
    } 
  }
   
  </script>
  <style scoped>
      div {
        text-align: left;
          float: right;
      }
  </style>