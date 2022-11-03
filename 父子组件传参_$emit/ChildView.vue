<template>
  <div class="child">
    <h2>子组件: {{a}}</h2>
    <button @click='change'>点击修改</button>
  </div>
</template>

<script>
export default {
  props: {
    a: {
      type: Number,
      require: true,
    }
  },
  data() {
    return {
      
    }
  },

  methods: {
    change() {
      let re = this.a + 1;
      this.$emit('gai',re)
    }
  }
}
</script>

<style>

</style>