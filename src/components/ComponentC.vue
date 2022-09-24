<template>
  <h1>component c</h1>
  <h2>userName by provide_Inject:{{ userName }}</h2>
  <button @click="add">click</button>
</template>

<script>
export default {
  inject: ["userName", "oneFunc"],
};
</script>

<style>
</style>