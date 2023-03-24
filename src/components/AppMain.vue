<script>
import AppNav from './AppNav.vue';
import ListApp from './ListApp.vue';
    export default{
        components:{
            AppNav,
            ListApp
        }
    }
</script>

<template>
    <main class="container">
        <div class="content">
            - Content goes Here -
        </div>
    </main>
    <AppNav></AppNav>
    <ListApp></ListApp>
</template>

<style lang="scss" scoped>
@use '../scss/variables.scss' as * ;
.container{
        height: 130px;
        color: $secondary;
        background-color:$primary;
}
</style>