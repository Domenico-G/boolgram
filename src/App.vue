<template>
  <div id="app">
    <header>
      <nav-component />
    </header>
    <main>
      <content-component />
      <sidebar />
    </main>
  </div>
</template>

<script>
import NavComponent from "./components/NavComponent.vue";
import ContentComponent from "./components/ContentComponent.vue";
import Sidebar from "./components/Sidebar.vue";

export default {
  name: "App",
  components: {
    NavComponent,
    ContentComponent,
    Sidebar,
  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@200;300;400;600;700;900&display=swap');

* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

main {
  @include container;
}

header {
  box-shadow: 0px 1px 4px 0px rgba(0, 0, 0, 0.46);
}

#app {
  font-family: 'Source Sans Pro', sans-serif;
  color: #2c3e50;
}
</style>
