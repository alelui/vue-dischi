<template>
    <div class="album">
        <img :src="info.poster" alt="">
        <h2>{{info.author}}</h2>
        <p>{{info.title}}</p>
        <p>{{info.year}}</p>
    </div>    
</template>

<script>
export default {
    name: 'album',
    props: {
        info: Object
    }
}
</script>

<style lang="scss" scoped>
    .album{
        background-color: #2e3a46;
        text-align: center;
        padding: 25px 18px 50px;
        font-size: 14px;

        img{
            width: 100%;
        }
        h2{
            color: white;
            margin: 15px 0;  
        }
        p{
            color: #596b76;
        }
    }
</style>