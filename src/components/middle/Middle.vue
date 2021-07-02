<template>
  <div>
    <div class="bbody">
      <middleleft></middleleft>
    </div>
  </div>
</template>

<script>
import middleleft from './middleleft/Middleleft'
export default {
  name: "",
  props: {},
  data() {
    return {};
  },
  components: {
    middleleft,
  },
  methods: {},
  mounted() {},
  computed: {},
  watch: {},
};
</script>

<style lang='scss' scoped>
.bbody {
  background: #e1e1e1;
}
</style>