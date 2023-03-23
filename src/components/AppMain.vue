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
@import "../scss/variables.scss";
.container{
        height: 130px;
        color: $secondary;
        background-color:$primary;
}
</style>