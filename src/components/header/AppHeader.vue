<script>
    export default{
        data(){
            return{
            menuItem:[
                {
                    menuName: 'CHARACTERS',
                    target: '_self'
                },
                {
                    menuName: 'COMICS',
                    target: '_self'
                },
                {
                    menuName: 'MOVIES',
                    target: '_self'
                },
                {
                    menuName: 'TV',
                    target: '_self'
                },
                {
                    menuName: 'GAMES',
                    target: '_self'
                },
                {
                    menuName: 'COLLECTIBLES',
                    target: '_self'
                },
                {
                    menuName: 'VIDEOS',
                    target: '_self'
                },
                {
                    menuName: 'FANS',
                    target: '_self'
                },
                {
                    menuName: 'NEWS',
                    target: '_self'
                },
                {
                    menuName: 'SHOP',
                    target: '_self'
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
                <img src="src/assets/img/dc-logo.png" alt="logo-dc">
            </div>  
            <div class="menu">
                <ul class="menu-list">
                    <li v-for="menu in menuItem">
                        <a href="#" target="{{menu.target}}">{{menu.menuName}}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../../styles/variables.scss' as * ;
    .container{
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        .logo,.menu{
            padding: 20px;
        }
        .menu .menu-list{
            list-style: none;
            display: flex;
        }
        li{
            padding: 15px;
            font-size: 12px;
            &:hover {
                color: $secondary;
                border-bottom: 5px solid $secondary;
            }
        }
        li a {
            color: $primary;
            text-decoration: none;
                &:hover{
                color: $secondary;
                }
        }
    }
</style>