<template>
  <div class="users-tips">
    <div class="img-nik-user">
      <img
        class="pic-user"
        src="../assets/img/profile.jpg"
        alt="Picture user"
      />
      <p>tess61</p>
    </div>
    <p>Segui</p>
  </div>
</template>

<script>
export default {
  name: "UsersTips",
  props: {},
};
</script>

<style lang="scss" scoped>
.users-tips {
  @include flex-center;
  margin: 15px 0;

  .img-nik-user {
    display: flex;
    align-items: center;

    p {
      font-weight: 600;
    }
    .pic-user {
      height: 40px;
      width: 40px;
      border-radius: 50%;
      margin-right: 15px;
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
