<template>
  <div id="app">
    <p>You're doctor</p>
    <p v-if="xacdinh">Yes, I am</p>
    <p v-else>No, I am not</p>

    <hr />
    <div id="wrap" v-if="xacdinh">
      <div>Menu 1</div>
      <div>Menu 1</div>
      <div>Menu 1</div>
      <div>Menu 1</div>
      <div>Menu 1</div>
    </div>
    <p v-show="xacdinh">Test show element</p>
    <button @click="changeXacdinh">Doi cau tra loi</button>
  </div>
</template>

<script>
// v-if se remove phan tu di, con v-show se an phan tu di

export default {
  name: "App",
  data() {
    return {
      xacdinh: true,
    };
  },
  methods: {
    changeXacdinh: function () {
      this.xacdinh = !this.xacdinh;
      return;
    },
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
