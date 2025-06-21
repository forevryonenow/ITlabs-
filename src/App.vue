<script>
    import ButtonLeftIcon from './components/ButtonLeftIcon.vue'
    import HeaderBarPrime from './components/HeaderbarPrime.vue'


    export default{
        components: { ButtonLeftIcon, HeaderBarPrime }
    }
</script>

<template>
    <header>
        <HeaderBarPrime />
    </header>
    
    <main>
        <div class="main-block">
            <ButtonLeftIcon />
            <ButtonLeftIcon />
            <ButtonLeftIcon />
            <ButtonLeftIcon />
            <ButtonLeftIcon />
            <ButtonLeftIcon />
            <ButtonLeftIcon />
            <ButtonLeftIcon />
            <ButtonLeftIcon />
        </div>
        
    </main>
</template>

<style scoped>
    .main-block{
        margin-top: 30px;
        display: grid;
        display:grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(3, 1fr);
        gap: 15px;
    }
</style>
