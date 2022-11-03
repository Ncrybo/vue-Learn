<template>
  <div class="home">
    <h2>父组件：{{num}}</h2>
    <child-view :a.sync="num" />
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
  }

}
</script>

<style>

</style>