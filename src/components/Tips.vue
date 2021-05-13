<template>
  <div class="suggerimenti">
    <div class="head-tips">
      <p>Suggerimenti per te</p>
      <p>Mostra tutti</p>
    </div>
    <users-tips v-for="item in 6" :key="item" />
  </div>
</template>

<script>
import UsersTips from './UsersTips.vue';


export default {
  name: 'Tips',
  components: {
    UsersTips
  },
  props: {

  }
}
</script>

<style lang="scss" scoped>
 
 .suggerimenti {
     margin-top: 70px;

     .head-tips {
       display: flex;
       justify-content: space-between;
       margin-bottom: 30px;
       color: gray;
       font-weight: 600;

       p:last-child {
         color: #000;
       }
     }
 }

</style>
