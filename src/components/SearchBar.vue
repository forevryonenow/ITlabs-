<template>
    <div class="con-search">
        <router-link to="/Search" class="router"><button class="search"><img src="/src/components/icons/lens white.svg" alt="">ПОИСК ГЕРОЯ</button></router-link>
        <button class="filter"><img src="/src/components/icons/favourites.svg" alt="">ФИЛЬТР</button>
        <h2>СТЕНА ПАМЯТИ</h2>
    </div>
</template>
<style scoped>
    .con-search{
        display: flex;
        align-items: center;
        gap: 20px;
        margin-top: 20px;
    }
    .router{
        text-decoration: none;
    }
    .search{
        display: flex;
        align-items: center;
        height: 69px;
        width: 280px;
        background-color: #CF3337;
        font-size: 18px;
        border: 0;
        color: #FFFFFF;
    }
    .filter{
        height: 69px;
        width: 280px;
        background: none;
        color: #514F4D;
        font-size: 18px;
        border: 1px solid #514F4D;
    }
    button{
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: pointer;
        text-transform: uppercase;
        text-decoration: none;
    }
    .search img{
        height: 25px;
        width: 25px;
        margin-right: 15px;
    }
    .filter img{
        height: 25px;
        width: 27px;
        margin-right: 15px;
    }
    h2{
        font-size: 40px;
        color: #514F4D;
    }
</style>

