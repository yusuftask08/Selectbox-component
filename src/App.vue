<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <h3>Select Box Component</h3>
    <SelectBox :data="data" />
  </div>
</template>

<script>
import SelectBox from './Components/Selectbox/index.vue'
import data from "./data/data.json";
export default {
  name: "App",
  components:{
    SelectBox
  },
  data() {
    return {
      data: data,
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>