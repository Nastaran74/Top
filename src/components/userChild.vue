<template>
  <div id="app">
    <p>parent Name is : {{ name }}</p>
    <p>parent ReverseName is : {{ reverseName() }}</p>
    <hr>
    <button @click="changeName">change Name</button>
  </div>
</template>

<script>
export default {
  props: {
    name:{
        type:String
    }
  },
  methods: {
      changeName:function(){
          this.name="change name to masi";
          this.$emit('changeName',this.name);
      } 
  },
//   methods: {
//     reverseName: function () {
//       return this.name.split("").reverse().join("");
//     },
//   },
};
</script>

<style scoped>
</style> 