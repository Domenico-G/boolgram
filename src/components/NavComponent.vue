<template>
  <div class="navbar">
    <div class="logo">
      <img alt="Boolgram logo" src="../assets/logo.png" />
    </div>
    <div class="search">
      <input type="text" placeholder="Cerca" />
    </div>
    <div class="settings-useer">
      <font-awesome-icon class="icon" :icon="['far', 'heart']" />
      <font-awesome-icon class="icon" :icon="['fas', 'home']" />
      <img
        class="pic-profile"
        src="../assets/img/profile.jpg"
        alt="Picture profile"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "NavComponent",
  props: {},
};
</script>

<style lang="scss" scoped>
.navbar {
  @include container;
  @include flex-center;
  padding: 10px 10px;

  // logo
  .logo {
    height: 40px;

    img {
      height: 100%;
    }
  }

  // input di ricerca
  .search {
    input {
      padding: 5px 20px;
      border: 1px solid #e6e6e6;
      &:focus {
        outline: 1px solid #a6a6a6;
      }

      &::placeholder {
        text-align: center;
      }
    }
  }

  // impostazioni utente
  .settings-useer {
    @include flex-center;
    width: 120px;

    .icon {
      font-size: 20px;
    }
  }
}

.pic-profile {
  height: 40px;
  width: 40px;
  border-radius: 50%;
}
</style>
