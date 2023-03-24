<script>
export default {
    name: 'Comics',
    props:{
        img: String,
        title: String
    }
}
</script>
<template>
    <div class="item">
        <div class="img">
            <img :src="img" alt="comic">
        </div>
        <h6>{{title}}</h6>
    </div>
</template>
<style lang="scss" scoped>
img {
    width: 100%;
    height: 150px;
    object-fit: content;
}
</style>