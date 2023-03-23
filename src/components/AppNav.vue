<script>
export default {
    data() {
        return {
            menuList: [
                {
                    item: 'DIGITAL COMICS',
                    imgPath:'public/img/buy-comics-digital-comics.png'
                },                
                {
                    item: 'DC MERCHANDISE',
                    imgPath:'/public/img/buy-comics-digital-comics.png'
                },
                {
                    item: 'SUBSCRIPTION',
                    imgPath:'./public/img/buy-comics-digital-comics.png'
                },
                {
                    item: 'COMIC SHOP LOCATOR',
                    imgPath:'./public/img/buy-comics-digital-comics.png'
                },
                {
                    item: 'DC POWER VISA',
                    imgPath:'./public/img/buy-comics-digital-comics.png'
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
                <a href="#">
                    <img :src="menu.imgPath" alt="img">
                    {{menu.item}}
                </a>
            </li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
@import "../scss/variables.scss";
nav{
    background-color: $secondary;
}
ul{
    list-style: none;
    display: flex;
}
</style>