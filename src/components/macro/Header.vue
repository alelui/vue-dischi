<template>
    <header>
        <nav>
            <i class="fab fa-spotify"></i>
            <input type="text" placeholder="Search" v-model="search" @keyup.enter="searchCharacter()">
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return{
            search: ''
        }
    },
    methods: {
        searchCharacter(){
            alert('hello!');
        }
    }
}
</script>

<style lang="scss" scoped>
    nav{
        height: 50px;
        background-color: #2e3a46;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;

        .fa-spotify{
            font-size: 37px;
            color: #1ed760;
        }

        input{
            padding: 5px;
            border: none;
            border-radius: 20px;
        }
    }
</style>