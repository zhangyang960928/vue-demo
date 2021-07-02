<template>
  <div>
    <div class="head">
      <topleft></topleft>
    </div>
  </div>
</template>

<script>
import topleft from "./topleft/TopLeft";
export default {
  name: "",
  props: {},
  data() {
    return {};
  },
  components: {
    topleft,
  },
  methods: {},
  mounted() {},
  computed: {},
  watch: {},
};
</script>

<style lang='scss' scoped>
.head {
  background: #444444;
  height: 50px;
}
</style>