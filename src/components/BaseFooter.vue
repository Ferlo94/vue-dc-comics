<template>
  <footer class="footer">
      <div class="footer__container">
        <div class="footer__top">
            <img src="../assets/img/buy-comics-digital-comics.png">
            <img src="../assets/img/buy-comics-merchandise.png">
            <img src="../assets/img/buy-comics-subscriptions.png">
            <img src="../assets/img/buy-comics-shop-locator.png">
            <img src="../assets/img/buy-dc-power-visa.svg">
        </div>

        <div class="footer__mid">

        </div>

        <div class="footer__bottom">

        </div>

      </div>
  </footer>
</template>

<script>
export default {
    name: 'BaseFooter'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/mixins.scss';

.footer {
    height: 150px;
    background-color: var(--primary-color);
    @include listInline;

    &__container {
        @include listInline;
        margin: auto;
        width: var(--container-md);
        align-items: center;
    }

    &__top {
        width: 100%;
        height: 150px;
        background-color: var(--primary-color);
        @include listInline;
        justify-content: space-between;

        img {
            max-width: 100%;
            max-height: 100%;
            margin: auto;
            padding: 35px;
        }
        
    }
}

</style>