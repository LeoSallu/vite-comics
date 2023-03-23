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
     <nav class="list-app">
        <ul>
            <li v-for="comics in dcComics">
                <div class="menu-container">
                    <div class="text">
                        <a href="#">{{comics.linkName}}</a>
                    </div>
                </div>
            </li>
        </ul>
        <ul>
            <li v-for="shopLink in shop">
                <div class="menu-container">
                    <div class="text">
                        <a href="#">{{shopLink.linkName}}</a>
                    </div>
                </div>
            </li>
        </ul>
        <ul>
            <li v-for="policy in dc">
                <div class="menu-container">
                    <div class="text">
                        <a href="#">{{policy.linkName}}</a>
                    </div>
                </div>
            </li>
        </ul>
        <ul>
            <li v-for="site in sites">
                <div class="menu-container">
                    <div class="text">
                        <a href="#">{{site.linkName}}</a>
                    </div>
                </div>
            </li>
        </ul>
    </nav>
</template>
<style lang="scss" scoped>
</style>