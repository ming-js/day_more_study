<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <div style="font-weight: normal;">{{ data.id }}</div>
  <div style="font-weight: bold;">{{ data.id }}</div>
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import { ref } from 'vue'
export default {
  name: 'App',
  // components: {
  //   HelloWorld
  // },
  /**
   * ref: 修改基础类型数据 -- el.value
   * 
   */
  setup() {
    const data = ref({
      id: 1,
      index: 2
    })

    return {
      data
    }
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
