<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <MyCounter />
</template>

<script>
import { defineAsyncComponent } from "@vue/runtime-core";

export default {
  name: "App",
  components: {
    MyCounter: defineAsyncComponent(() => import("@/components/MyCounter.vue")),
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
