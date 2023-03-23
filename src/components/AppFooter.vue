<script>
    export default{
        data(){
            return{
                icon:[
                    {
                        pathImg:'/public/img/footer-facebook.png'
                    },
                    {
                        pathImg:'/public/img/footer-twitter.png'
                    },
                    {
                        pathImg:'/public/img/footer-youtube.png'
                    },
                    {
                        pathImg:'/public/img/footer-pinterest.png'
                    },
                    {
                        pathImg:'/public/img/footer-periscope.png'
                    }
                ]
            }
        }
    }
</script>

<template>
    <footer>
        <div class="container">
            <div class="button">
                <h3>SIGN-UP NOW!</h3>
            </div>
            <div class="list-container">
                <ul>
                   <li><h3>FOLLOW US</h3></li>
                   <li v-for="icons in icon">
                        <div class="img">
                            <img :src="icons.pathImg" alt="logo">
                        </div>
                   </li> 
                </ul>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@import "../scss/variables.scss";
    footer{
        background-color: $primary;
        padding: 10px;
        .container{
            display: flex;
            justify-content: space-between;
            align-items:center;
        }
        ul{
            list-style: none;
            display: flex;
            align-items: center;
        }
        h3{
            color: $secondary;
            cursor: pointer;
        }
        .list-container ul{
            display: flex;
        }
        li{
            padding: 10px;
        }
    }
    .button{
        text-align: center;
        width: 200px;
        padding: 20px;
        border: 3px solid $secondary;
        h3{
            color: white;
            cursor: pointer;
        }
    }

</style>