<!--test.vue-->
<template>
  <div class="xu-test" @click="handleClick">{{ num }}</div>
</template>

<script>
export default {
  name: 'XuTest', // 这个名字很重要，它就是未来的标签名<xr-test></xr-test>，坑了我一下
  data () {
    return {
      num: 0
    }
  },
  methods: {
    handleClick () {
      this.num++
    }
  }
}
</script>
