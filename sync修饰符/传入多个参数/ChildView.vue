<template>
  <div class="child">
    <h2>我是子组件</h2>
    <p>我也叫{{name}}，今年{{age}}岁</p>
    <button @click='$emit("update:name","小明")'>点击修改</button>
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    age: Number,
  },
  data() {
    return {
      
    }
  },

  methods: {
  }
}
</script>

<style>

</style>