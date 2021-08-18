<template>
  <div>
    Child:{{ msg1 }}
  </div>
</template>
<script>
export default {
  name: "Child",
  props: {
    msg1: {
      type: String,
      default: "",
    },
  },
  data() {
    return {
      msg2: "子组件再传数据给父组件",
    };
  },
  mounted: function () {
    this.$emit("getMessage", this.msg2);
  },
};
</script>