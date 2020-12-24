<template>
  <div id="app">
    <h1>Parent: {{pizzaName}}</h1>
    <app-pizza v-bind:pizzaName='pizzaName' v-bind:pizzaPrice='pizzaPrice'>
      <h1> С Новым годом! </h1>
      <h2 slot='n1'>Покупайте пиццу</h2>
    </app-pizza>
  </div>
</template>
<script>
  import Pizza from './components/Pizza.vue'

  export default {
    name: 'app',
    data() {
      return {
        pizzaName: 'ШПицца от Школы программистов',
        pizzaPrice: 600

      }
    },
    components: {
      appPizza: Pizza
    }
  }
</script>
<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>