<template>
  <div>
    <Parnets></Parnets>
  </div>
</template>

<script>
import Parnets from "~/components/Parents.vue";
import { computed } from "vue";

export default {
  name: "IndexPage",
  components: {
    Parnets,
  },
  data() {
    return {
      user: {
        name: null,
        age: null,
        type: null,
      },
    };
  },
  provide() {
    return {
      user: computed(() => this.user),
    };
  },
  mounted() {
    this.user = {
      name: "홍길동",
      age: 20,
      type: 3,
    };
  },
};
</script>
