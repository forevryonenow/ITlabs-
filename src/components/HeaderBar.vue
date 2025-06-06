<template>
    <header :class="{'font-color' : another}">
        <img src="/src/assets/лого.png" alt="">
        <div class="text">
            <h1>Музей Боевой и Трудовой Славы</h1>
            <h2>город Александров</h2>
        </div>
    </header>
</template>
<script>
    export default {
        props: {
            another: {
                type: Boolean,
                default: false
            }
        }
    }
</script>
<style scoped>
    header{
        display: flex;
        align-items: center;
        justify-content: left;
    }
    img{
        width: 86px;
        margin-right: 20px;
    }
    h1{
        color: #2B2A29;
        font-size: 64px;
    }
    h2{
        color: #514F4D;
        font-size: 58px;
        margin: 0;
    }
</style>