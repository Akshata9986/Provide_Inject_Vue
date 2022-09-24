<template>
  <component-a />
</template>

<script>
import ComponentA from "./components/ComponentA.vue";

export default {
  name: "App",
  components: {
    ComponentA,
  },
  data() {
    return {
      userName: "Raju Rastogi",
    };
  },
  methods: {
    add() {
      console.log("add is exicuted");
    },
  },
  provide() {
    return {
      userName: this.userName,
      oneFunc: this.add,
    };
  },
};
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