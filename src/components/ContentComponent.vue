<template>
  <div class="content">
    <div class="story-container">
      <story v-for="item in 6" :key="item" />
    </div>
    <post v-for="item in 3" :key="item" />
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

<style lang="scss" scoped>
.content {
  width: 60%;

  .story-container {
    @include flex-center;
    overflow: hidden;
    border: 1px solid #e6e6e6;
    border-radius: 5px;
    padding: 30px 30px;
  }
}
</style>
