<script>
    export default{
        data(){
            return{
                dcComics:[
                    {
                        linkName: 'Character'
                    },
                    {
                        linkName: 'Comics'
                    },
                    {
                        linkName: 'Movies'
                    },
                    {
                        linkName: 'TV'
                    },
                    {
                        linkName: 'Games'
                    },
                    {
                        linkName: 'Videos'
                    },
                    {
                        linkName: 'News'
                    }
                ],
                shop:[
                    {
                        linkName: 'Shop DC'
                    },
                    {
                        linkName: 'Shop DC Collectibles'
                    }
                ],
                dc:[
                    {
                        linkName: 'Terms of Use'
                    },
                    {
                        linkName: 'Privacy Police'
                    },
                    {
                        linkName: 'Ad Choices'
                    },
                    {
                        linkName: 'Advertising'
                    },
                    {
                        linkName: 'Jobs'
                    },
                    {
                        linkName: 'Subscriptions'
                    },
                    {
                        linkName: 'Talent Workshops'
                    },
                    {
                        linkName: 'Ratings'
                    },
                    {
                        linkName: 'Shop Help'
                    },
                    {
                        linkName: 'Contact us'
                    }
                ],
                sites:[
                    {
                        linkName: 'DC'
                    },
                    {
                        linkName: 'MAD Magazine'
                    },
                    {
                        linkName: 'DC kids'
                    },
                    {
                        linkName: 'DC Universe'
                    },
                    {
                        linkName: 'DC Power Visa'
                    }
                ]
            }
        }
    }
</script>
<template>
    <nav>
        <div class="list-app-left">
                <ul>
                    <li><h4>DC COMICS</h4></li>
                    <li v-for="comics in dcComics">
                        <div class="menu-container">
                            <div class="text">
                                <a href="#">{{comics.linkName}}</a>
                            </div>
                        </div>
                    </li>
                </ul>
                <ul>
                    <li><h4>SHOP</h4></li>
                    <li v-for="shopLink in shop">
                        <div class="menu-container">
                            <div class="text">
                                <a href="#">{{shopLink.linkName}}</a>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
        <div class="list-app-mid">
            <ul>
                <li><h4>DC</h4></li>
                <li v-for="policy in dc">
                    <div class="menu-container">
                        <div class="text">
                            <a href="#">{{policy.linkName}}</a>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
        <div class="list-app-right">
            <ul>
                <li><h4>SITES</h4></li>
                <li v-for="site in sites">
                    <div class="menu-container">
                        <div class="text">
                            <a href="#">{{site.linkName}}</a>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </nav>
</template>
<style lang="scss" scoped>
    nav{
        display: flex;
        padding: 20px;
        background-image: url('public/img/footer-bg.jpg');
        background-size: cover;
        h4{
            color: white;
        }
        ul{
            list-style: none;
        }
        a{
            color: #959595;
            text-decoration: none;
        }
    }
</style>