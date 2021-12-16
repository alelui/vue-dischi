<template>
    <div>
       <div class="container">
           <div class="row">
               <album/>
           </div>
            <div class="row">
               <album/>
           </div>
       </div>
    </div>
</template>

<script>
import axios from 'axios';
import album from '../commons/album.vue';
export default {
    name: 'albums',
    components: {
        album
    }

}
</script>

<style lang="scss" scoped>
    .container{
        width: 80%;
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        
        .row{
            display: flex;
            flex-wrap: wrap;
            width: calc(100% / 5 - 40px);
            margin: 14px 20px;
        }
    }
</style>