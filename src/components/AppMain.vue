<script>
import AppNav from './AppNav.vue';
    export default{
        components:{
            AppNav
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

</template>

<style lang="scss" scoped>
@import "../scss/variables.scss";
.container{
        height: 130px;
        color: $secondary;
        background-color:$primary;
}
</style>