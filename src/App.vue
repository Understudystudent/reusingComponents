<template>
  <div class="container">
    <h1>App Component</h1>
    <input type="text" placeholder="Say something" v-model="msg">
    <Products :greeting="msg"/>
    <!-- <Products greeting="Class 1"/> -->
  </div>
</template>
<script>
import Products from './components/Product.vue';
export default {
  name: 'App',
  data() {
    return {
      msg: ''
    }
  },
  components: {
    Products
  }
}
</script>
<!-- Global styling -->
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2C3E50;
  margin-top: 60px;
}
.container {
  background-color: black;
}
</style>