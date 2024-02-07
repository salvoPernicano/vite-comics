<script>
import AppNavbar from './components/AppNavbar.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
    components: {
        AppNavbar,
        AppMain,
        AppFooter
    }
}
</script>

<template>
    <AppNavbar />
    <AppMain/>
    <AppFooter/>
</template>

<style lang="scss">
@use './styles/general.scss' ;
</style>
