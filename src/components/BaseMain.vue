<template>
  <main class="main">
    <div class="main__container">
        <div class="main__hero"></div>
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
    height: 400px;
    justify-content: center;

    

    &__container {
        @include listInline;
        margin: auto;
        width: 100%;
        // max-width: var(--container-md);
        align-items: center;
        
        

        h2 {
            color: var(--white);
        }


    }

    &__hero {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        width: 100%;
        height: 400px;
    }
}

</style>