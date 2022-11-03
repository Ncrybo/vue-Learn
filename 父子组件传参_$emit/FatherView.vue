<template>
  <div class="home">
    <h2>父组件：{{num}}</h2>
    <child-view :a="num" @gai="change()" />
    <!-- <child-view :a="num" @gai="change(val)" />  错误的写法 -->
  </div>
</template>

<script>
import ChildView from '@/views/ChildView.vue'

export default {
  name: 'FatherView',
  components: {ChildView},
  data() {
    return {
      num: 10,
    }
  },

  methods: {
    change(val) {
      this.num = val
    }
  }

}
</script>

<style>

</style>