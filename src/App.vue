<template>
  <div id="app">
     <v-header></v-header>
     <v-logo></v-logo>
     <v-nav></v-nav>
     <transition  name="custom-classes-transition"
                  enter-active-class="animated tada"
                  leave-active-class="animated bounceOutRight">
         <router-view></router-view>
     </transition>
     <v-footer></v-footer>
  </div>
</template>

<style>
</style>

<script>
  import header from  './components/header/head.vue';
  import logo from './components/logo/logo.vue';
  import nav from './components/Navigation/nav.vue';
  import footer from './components/footer/footer.vue';

  export default {
      data() {
         return {
         }
      },
     components: {
       'v-header':header,     //注册组件
       'v-logo':logo,
       'v-nav':nav,
       'v-footer':footer
     }
  }
</script>

