<template>
    <section class="search-page">
        <header>
            <HeaderBar another />
        </header>
        <main>
            <h2 class="search-hero">ПОИСК ПО БАЗЕ ГЕРОЕВ</h2>
            <div class="container-search">
                <input class="inp-search" type="search" name="" id="" placeholder="Кого вы ищите?">
                <button class="btn-lens" type="submit"><img src="/src/components/icons/lens white.svg" alt=""></button>
            </div>
            <div class="btn-link">
                <router-link to="/"><button class="btn">НА ГЛАВНУЮ</button></router-link>
            </div>
        </main>
    </section>
</template>
<script>
    import HeaderBar from './HeaderBar.vue'
    import VirtualKeyboard from './VirtualKeyboard.vue'
    export default{
        components: {HeaderBar, VirtualKeyboard}
    }
</script>
<style>
    .search-page{
        background-size: cover;
        background-repeat: no-repeat;
        background-color: rgba(0, 0, 0, 0.5);
        background-blend-mode: multiply;        
        margin-top: -80px;
        margin-left: -80px;
        min-height: 100vh;
        padding: 80px;
    }
    .search-hero{
        margin-top: 125px;
        margin-bottom: 50px;
        font-size: 40px;
        color: #FFFFFF;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .container-search{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .inp-search{
        width: 873px;
        height: 80px;
        border-bottom: 2px solid #C1A886;
        border-top: none;
        border-left: none;
        border-right: none;
        background-color: transparent;
        font-size: 32px;
        font-style: italic;
        color: #FFFFFF;
    }
    .btn-lens{
        background: none;
        border: none;
        cursor: pointer;
        width: 40px;
        height: 40px;
        position: relative;
        right: 65px;
    }
    .main{
        margin-top: 100px;
        background: none;
        cursor: pointer;
        border: 1px solid #FFFFFF;
        width: 576px;
        height: 69px;
        color: #FFFFFF;
        font-size: 18px;
    }
    .btn-link{
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 100px;
    }
    .btn{
        width: 576px;
        height: 69px;
        background-color: transparent;
        border: 1px solid #FFFFFF;
        color: #FFFFFF;
        font-size: 18px;
    }
    input::-webkit-search-cancel-button{
        display: none;
    }
    ::-webkit-input-placeholder{
        color:    #FFFFFF;
        font-style: italic;
    }
</style>