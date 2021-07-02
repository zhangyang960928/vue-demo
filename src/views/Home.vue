<template>
  <div>
    <div class="wrod">
      <top></top>
      <middle></middle>
      <foot></foot>
    </div>
  </div>
</template>

<script>
import top from "../components/top/Top";
import middle from "../components/middle/Middle";
import foot from "../components/foot/Foot";
export default {
  name: "",
  props: {},
  data() {
    return {};
  },
  components: {
    top,
    middle,
    foot,
  },
  methods: {},
  mounted() {},
  computed: {},
  watch: {},
};
</script>

<style lang='scss' scoped>
.wrod {
  background: #e1e1e1;
}
</style>
