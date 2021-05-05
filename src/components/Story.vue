<template>
  <div class="story">
    <div class="story-pic">
      <img src="../assets/img/profile.jpg" alt="" />
    </div>
    <p>trunte</p>
  </div>
</template>

<script>
export default {
  name: "Story",
  props: {},
};
</script>

<style lang="scss" scoped>
.story {
  // margin-left: 20px;
  text-align: center;

  .story-pic {
    width: 60px;
    height: 60px;
    border: 2px solid red;
    border-radius: 50%;
    padding: 1px;

    img {
      border-radius: 50%;
      width: 100%;
    }
  }

  p {
    margin-top: 6px;
    font-size: 12px;
    font-weight: 700;
    color: #1a1a1a;
  }
}
</style>
