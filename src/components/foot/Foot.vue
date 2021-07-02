<template>
  <div>
    <div class='foot'><footword></footword></div>
  </div>
</template>

<script>
import footword from './footword/Footword'
export default {
  name: '',
  props:{},
  data () {
    return {
    }
  },
  components: {
    footword
  },
  methods: {},
  mounted() {},
  computed: {},
  watch: {}
}
</script>

<style lang='scss' scoped>
.foot {
  background: #ffffff;
}
</style>