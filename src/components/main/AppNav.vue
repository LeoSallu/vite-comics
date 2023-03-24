<script>
export default {
    data() {
        return {
            menuList: [
                {
                    item: 'DIGITAL COMICS',
                    imgPath:'./src/assets/img/buy-comics-digital-comics.png'
                },                
                {
                    item: 'DC MERCHANDISE',
                    imgPath:'./src/assets/img/buy-comics-merchandise.png'
                },
                {
                    item: 'SUBSCRIPTION',
                    imgPath:'./src/assets/img/buy-comics-subscriptions.png'
                },
                {
                    item: 'COMIC SHOP LOCATOR',
                    imgPath:'./src/assets/img/buy-comics-shop-locator.png'
                },
                {
                    item: 'DC POWER VISA',
                    imgPath:'./src/assets/img/buy-dc-power-visa.svg'
                }
            ]
        }
    }
}
</script>

<template>
    <nav class="menu">
        <ul>
            <li v-for="menu in menuList">
                <div class="menu-container">
                    <div class="img">
                        <img :src="menu.imgPath" alt="img">
                    </div>
                    <div class="text">
                        <a href="#">{{menu.item}}</a>
                    </div>
                </div>
            </li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
    @import "../../styles/variables.scss";
    nav{
        display: flex;
        justify-content: center;
        padding: 20px;
        background-color: $secondary;
    }
    .menu-container{
        display: flex;
        align-items: center;
        cursor: pointer;
        padding: 10px;
            a{
                color: white;
                text-decoration: none;
                &:hover{
                    border-bottom: 2px solid white;
                }
            }
            .img{
                width: 60px;
                padding: 5px;
            }
            img{
                width: 100%;
                display: block;
                object-fit:center;
            }
    }
    ul{
        list-style: none;
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>