<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <div class="border">
            <h1>{{ msg }}</h1>
            <h2>Hi</h2>
            <hr>
            <helloWorld></helloWorld>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import helloWorld from "./components/HelloWorld.vue";
export default {
  name: "App",
  data() {
    return {
      msg: "salam azizam",
    };
  },
  components: {
    helloWorld,
  },
};
</script>

<style scoped>
.container {
  background-color: bisque;
  height: 1000px;
  width: 530px;
  display: flex;
}
.row {
  background-color: burlywood;
  height: 350px;
  width: 350px;
  margin: 50px 50px;
}
.border {
  background-color: chocolate;
  height: 150px;
  width: 150px;
  margin: 50px 50px;
}
.border h1 {
  font-size: 20px;
}
</style>