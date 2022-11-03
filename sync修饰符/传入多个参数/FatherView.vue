<template>
  <div class="home">
    <h2>我是父组件</h2>
    <p>我叫{{person.name}}, 今年{{person.age}}岁</p>
    <br/>
    <!-- 传入多个参数的写法 -->
    <child-view v-bind.sync="person" />
  </div>
</template>

<script>
import ChildView from '@/views/ChildView.vue'

export default {
  name: 'FatherView',
  components: {ChildView},
  data() {
    return {
      person: {
        name:'mike',
        age: 15,
      }
    }
  },

  methods: {
  }

}
</script>

<style>

</style>