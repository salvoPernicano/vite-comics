<script>
import AppNavbar from './components/AppNavbar.vue';
import AppMain from './components/AppMain.vue'
export default {
    components: {
        AppNavbar,
        AppMain
    }
}
</script>

<template>
    <AppNavbar />
    <AppMain/>
</template>

<style lang="scss">
@use './styles/general.scss' ;
body{
    background-color: aqua;
    height: 100vh;
}
</style>
