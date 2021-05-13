<template>
  <div class="sidebar">
    <user-profile />
    <tips />
    <footer>
      <p>© 2021 Instagram from facebook</p>
    </footer>
  </div>
</template>

<script>
import UserProfile from "./UserProfile.vue";
import Tips from "./Tips.vue";

export default {
  name: "Sidebar",
  components: {
    UserProfile,
    Tips,
  },
  props: {},
};
</script>

<style lang="scss" scoped>
.sidebar {
  width: 40%;
  padding: 20px 0px 0px 50px;


  footer {
    margin-top: 50px;
    color: #cccccc;
    font-weight: 600;
    text-transform: uppercase;
  }
}

</style>
