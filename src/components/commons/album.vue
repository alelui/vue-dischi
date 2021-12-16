<template>
    <div class="album">
        <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
        <h2>New Jersey</h2>
        <p>Bon Jiovi</p>
        <p>1968</p>
    </div>    
</template>

<script>
export default {
    name: 'album'
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