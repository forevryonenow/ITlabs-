<template>
    <div>
        <header>
            <HeaderBar />
        </header>
        <main>
            <SearchBar />
            <HeroCard />
            <router-view></router-view>
        </main>
    </div>
</template>
<script>
    import HeaderBar from './HeaderBar.vue'
    import SearchBar from './SearchBar.vue'
    import HeroCard from './HeroCard.vue'
    export default{
        components: { HeaderBar, SearchBar, HeroCard }
    }

</script>