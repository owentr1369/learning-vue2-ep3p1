<template>
  <div id="app">
    <p>You're doctor</p>
    <p v-if="xacdinh">Yes, I am</p>
    <p v-else>No, I am not</p>
    <button @click="changeXacdinh">Doi cau tra loi</button>
  </div>
</template>

<script>
// Tat ca du lieu truyen qua html o dang du lieu tho
// computed thuc hien nhu mot function nhung chi duoc coi la 1 t
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
