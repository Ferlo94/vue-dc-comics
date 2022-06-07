<template>
  <main class="main">
    <div class="main__container">
        <div class="main__hero"></div>
        <div class="main__bottom">
            <div class="main__container-2">
                <div class="films" v-for="i in 12" :key="i"></div>
            </div>
        </div>
    </div>
        
  </main>
</template>

<script>
export default {
    name: 'BaseMain'
}
</script>

<style lang='scss' scoped>
@import '../assets/style/mixins.scss';

.main {
    @include listInline;
    height: 800px;
    justify-content: center;
    

    

    &__container {
        @include listInline;
        margin: auto;
        width: 100%;
        
        flex-direction: column;
        
        

        h2 {
            color: var(--white);
        }


    }

    &__container-2 {
        max-width: var(--container-md);
        @include listInline;
        flex-wrap: wrap;
        // background-color: aqua;
        height: 100%;
        margin: auto;
        align-items: center;
        justify-content: center;

    }

    &__hero {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        width: 100%;
        height: 300px;
    }

    &__bottom {
        height: 500px;
        width: 100%;
        background-color: black;

    }

    .films {

        width: calc(15%);
        height: 200px;
        margin: 5px;
        background-color: white;
    }
}

</style>