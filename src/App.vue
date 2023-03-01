<script>
import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppMerch from './components/AppMerchFooter.vue.vue'
export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
    AppMerch,
  }
}
</script>

<template>
  <div>
    <AppHeader />
    <AppMain />
    <AppMerch />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use './style/general.scss';
</style>