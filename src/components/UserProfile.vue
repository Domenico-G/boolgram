<template>
  <div class="user-profile">
    <img
      class="pic-profile"
      src="../assets/img/profile.jpg"
      alt="Picture profile"
    />
    <div class="nikname-profile">
      <p>domenico grasso</p>
      <p>Domenico Grasso</p>
    </div>
    <p>Passa a</p>
  </div>
</template>

<script>
export default {
  name: "UserProfile",
  props: {},
};
</script>

<style lang="scss" scoped>
.user-profile {
  @include flex-center;


  .pic-profile {
    height: 45px;
    width: 45px;
    border-radius: 50%;
  }

  .nikname-profile {
    font-weight: 600;

    p:last-child {
      font-weight: 500;
      color: gray;
    }
  }

  > p {
    color: #4da6ff;
      font-size: 15px;
      font-weight: 600;
      cursor: pointer;
  }
}
</style>
