<template>

  <header class="header">

    <div class="header__logo">
      <img src="../assets/img/dc-logo.png">
    </div>

    <nav class="header__nav">
      <ul>
        <li class="active"><a href="#">CHARACTERS</a></li>
        <li class="active"><a href="#">COMICS</a></li>
        <li class="active"><a href="#">MOVIES</a></li>
        <li class="active"><a href="#">TV</a></li>
        <li class="active"><a href="#">GAMES</a></li>
        <li class="active"><a href="#">COLLECTIBLES</a></li>
        <li class="active"><a href="#">VIDEOS</a></li>
        <li class="active"><a href="#">FANS</a></li>
        <li class="active"><a href="#">NEWS</a></li>
        <li class="active"><a href="#">SHOP</a></li>
      </ul>
    </nav>

  </header>

</template>

<script>
export default {
    name: 'BaseHeader'
}
</script>



<style lang="scss" scoped>
@import '../assets/style/mixins.scss';

  .header {
    
    @include listInline;
    align-items: center;
    background-color: white;
    height: 150px;
    justify-content: space-around;

    &__logo {
      
    }

    &__nav {
       

      ul {

        @include listInline;

        a {
          color: var(--terzo-color);
          margin: .625rem;
          padding-bottom: 60px;
          text-decoration: none;
        }
        .active a:hover {
          border-bottom: 5px solid var(--primary-color);
          color: var(--primary-color);
        }
        

      }

      



    }
  }
</style>