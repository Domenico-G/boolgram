<template>
  <div class="">
    <user-profile />
    <typs />
    <footer-component />
  </div>
</template>

<script>
import UserProfile from "./UserProfile.vue";
import Typs from "./Typs.vue";
import FooterComponent from "./FooterComponent.vue";
export default {
  name: "Sidebar",
  components: {
    UserProfile,
    Typs,
    FooterComponent
  },
  props: {},
};
</script>

<style lang="scss" scoped></style>
