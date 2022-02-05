<template>
  <div class="hello">
    <h1>name:{{ userName }}</h1>
    <userChild :name="userName"></userChild>
    <button @click="changeUserName">changeNumber</button>
  </div>
</template>

<script>
import userChild from "./userChild.vue";
export default {
  components: { userChild },
  name: "HelloWorld",
  data() {
    return {
      userName: "Nasi",
   
    };
  },
  methods: {
    changeUserName:function(){
      this.userName="Nabi";
    }
  },
};
</script>

<style scoped>
</style>