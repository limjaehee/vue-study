<template>
  <div>
    💡메시지 필독
    <Child></Child>
  </div>
</template>

<script>
import Child from "~/components/Child.vue";

export default {
  name: "VueStudyParents",
  components: { Child },
};
</script>

<style lang="scss" scoped></style>
