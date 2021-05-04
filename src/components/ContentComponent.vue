<template>
  <div class="">
    <story />
    <post />
  </div>
</template>

<script>

import Story from "./Story.vue";
import Post from "./Post.vue";

export default {
  name: "ContentComponent",
  components: {
    Story,
    Post,
  },
  props: {},
};
</script>

<style lang="scss" scoped></style>
