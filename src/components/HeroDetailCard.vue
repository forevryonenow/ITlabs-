<template>
    
  <section>
    <header>
        <HeaderBar another />
    </header>
    <hr>
    <main class="hero-page">
        <div class="section-text">
            <h3 class="name">Абрамов Александр Степанович</h3>
            <div class="grid-text">
                <div class="year">
                    <h4>Год рождения</h4>
                    <p>1912г</p>
                </div>
                <div class="place">
                    <h4>Место рождения</h4>
                    <p>г. Орехово-Зуево Московская область</p>
                </div>
                <div class="rank">
                    <h4>Звание</h4>
                    <p>Старшина</p>
                </div>
                <div class="army">
                    <h4>Призван в армию</h4>
                    <p>01.08.1942</p>
                </div>
                <div class="death">
                    <h4>Как погиб</h4>
                    <p>Погиб в бою</p>
                </div>
                <div class="place-death">
                    <h4>Место гибели (захоронения)</h4>
                    <p>Смоленская обл.</p>
                </div>
                <div class="data-death">
                    <h4>Дата гибели</h4>
                    <p>Март 1942г</p>
                </div>
            </div>
            <div class="btn-page-hero">
                <router-link to="/" class="router"><button class="home">На главную</button></router-link>
                <button class="next-hero">
                <img src="/src/components/icons/medal.svg" alt="Орден">
                Следующий герой
                </button>
            </div>
            <span>Для стены памяти информация получена от родных, близких и друзей героев</span>
        </div>
      <div class="img">
          <img class="img-hero" src="@/assets/Георгий Прокофьевич Хлебородов.svg" alt="Абрамов Александр Степанович">
        </div>
    </main>
  </section>
</template>
<script>
    import HeaderBar from './HeaderBar.vue'
    export default{
        components: {HeaderBar}
    }
</script>
<style scoped>
hr{
    width: 1760px;
    margin-top: 48px;
    margin-bottom: 44px;
}
.hero-page{
    display: flex;
    flex-direction: row;
    gap: 400px;
    margin-top: 20px;
}
.name{
    font-size: 48px;
}
.grid-text{
    display: grid;
    grid-template-columns: repeat(3, 264px);
    row-gap: 20px;
    column-gap: 72px;
    margin-top: 40px;
}
h4{
    font-style: italic;
    font-size: 32px;
}
p{
    font-size: 24px;
}
.place{
    grid-column: span 2;
}
.place-death{
    grid-column: span 2 ;
}
.btn-page-hero{
    display: flex;
    align-items: center;
    gap: 16px;
    margin-top: 111px;
}
.home{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 428px;
    height: 69px;
    gap: 11px;
    font-size: 18px;
    border: 1px solid #514F4D;
    background-color: transparent;
}
.router{
    text-decoration: none;
}
.next-hero{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 16px;
    font-size: 18px;
    width: 428px;
    height: 69px;
    border-color: transparent;
    background-color: #CF3337;
}
span{
    font-size: 18px;
}
</style>