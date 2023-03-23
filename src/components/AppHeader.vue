<script>
    export default{
        data(){
            return{
            menuItem:[
                {
                    menuName: 'CHARACTERS'
                },
                {
                    menuName: 'COMICS'
                },
                {
                    menuName: 'MOVIES'
                },
                {
                    menuName: 'TV'
                },
                {
                    menuName: 'GAMES'
                },
                {
                    menuName: 'COLLECTIBLES'
                },
                {
                    menuName: 'VIDEOS'
                },
                {
                    menuName: 'FANS'
                },
                {
                    menuName: 'NEWS'
                },
                {
                    menuName: 'SHOP'
                }
            ]
        }
        }
    }
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="public/img/dc-logo.png" alt="logo-dc">
            </div>  
            <div class="menu">
                <ul class="menu-list">
                    <li v-for="menu in menuItem">
                        {{menu.menuName}}
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    .container{
        display: flex;
        justify-content: space-between;
        width: 700px;
        margin: 0 auto;
        .logo,.menu{
            padding: 10px;
        }
        .menu .menu-list{
            list-style: none;
            display: flex;
        }
    }
</style>