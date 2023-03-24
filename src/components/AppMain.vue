<script>
import JumboTron from './JumboTron.vue';
import ComicsShop from './ComicsShop.vue';
import AppNav from './AppNav.vue';
import ListApp from './ListApp.vue';
    export default{
        components:{
            AppNav,
            ListApp,
            JumboTron,
            ComicsShop
        }
    }
</script>

<template>
    <main>
        <JumboTron />
        <ComicsShop />
        <AppNav />
        <ListApp />
    </main>
</template>
