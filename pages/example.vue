<template>
    <div>
      <ExampleComponent @sendTopage="data_from = $event"/>
      <h1>Это страница - родитель</h1>
      <p>Это данные из компонента <b>{{ data_from }}</b></p>
    </div>
  </template>

  <script>
  import ExampleComponent from "@/components/ExampleComponent";
  export default {
    components: {
      ExampleComponent
    },
    data() {
      return {
        data_from: ""
      }
    }
  }
  </script>

  <style scoped>

  </style>