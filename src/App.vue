<script >
// import AppNav from './components/AppNav.vue'
import AppNav from './components/AppNav.vue' ;
import AppListing from './components/AppListing.vue';
import AppPay from './components/AppPay.vue';
import AppFooter from './components/AppFooter.vue';
import AppSocial from './components/AppSocial.vue';

export default {
  name: 'App',
  components: {
    AppNav,
    AppListing,
    AppPay,
    AppFooter,
    AppSocial
  }
}
</script>

<template>
  
  <AppNav />
  <AppListing />
  <AppPay />
  <AppFooter />
  <AppSocial />

</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $primary;
}
</style>