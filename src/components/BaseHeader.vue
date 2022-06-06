<template>

  <header class="header">

    <div class="header__logo">
      <img src="../assets/img/dc-logo.png">
    </div>

    <nav class="header__nav">
      <ul>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
        <li class="active"><a href="#">Link</a></li>
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

    &__logo {
      width: 30%;
    }

    &__nav {
       width: 60%;

      ul {

        @include listInline;

        a {
          color: var(--terzo-color);
          margin: .625rem;
          text-decoration: none;
        }
        .active a:hover {
          border-bottom: 5px solid var(--primary-color);

        }
        

      }

      



    }
  }
</style>