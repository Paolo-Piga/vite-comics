<script >
import AppNav from './components/AppNav.vue'
import AppContent from './components/AppContent.vue'
import AppPurchase from './components/AppPurchase.vue'
import AppFooter from './components/AppFooter.vue'
import AppSocial from './components/AppSocial.vue'

export default {
  name: 'App',
  components: {
    AppNav,
    AppContent,
    AppPurchase,
    AppFooter,
    AppSocial
  }
}
</script>

<template>
  
  <AppNav />
  <AppContent />
  <AppPurchase />
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