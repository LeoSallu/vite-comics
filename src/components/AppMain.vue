<script>
import JumboTron from './JumboTron.vue';
import AppNav from './AppNav.vue';
import ListApp from './ListApp.vue';
    export default{
        components:{
            AppNav,
            ListApp,
            JumboTron
        }
    }
</script>

<template>
    <main>
        <JumboTron />
        <AppNav />
        <ListApp />
    </main>
</template>

<style lang="scss" scoped>
    @use '../scss/variables.scss' as * ;
</style>