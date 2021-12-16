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
    },

    data(){
        return{
            albums: null
        }
    },

    created(){
        // Make a request for a user with a given ID
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then(function (response) {
            // handle success
            console.log(response);
        })
        .catch(function (error) {
            // handle error
            console.log(error);
        })
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