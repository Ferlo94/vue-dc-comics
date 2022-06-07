<template>
    <footer class="footer">
        <div class="footer__container">
            <div class="footer__top">
                <img src="../assets/img/buy-comics-digital-comics.png">
                <p>PROVA</p>
                <img src="../assets/img/buy-comics-merchandise.png">
                <p>PROVA</p>
                <img src="../assets/img/buy-comics-subscriptions.png">
                <p>PROVA</p>
                <img src="../assets/img/buy-comics-shop-locator.png">
                <p>PROVA</p>
                <img src="../assets/img/buy-dc-power-visa.svg">
                <p>PROVA</p>
            </div>
        </div>
        <div class="footer__mid">
            <div class="footer__container">
                <div class="footer__sx">
                    <div class="text-footer"><h3><strong class="white">DC COMICS</strong></h3><br><span class="grey">Lorem ipsum dolor sit amet consectetur</span></div>
                    <div class="text-footer"><h3><strong class="white">DC COMICS</strong></h3><br><span class="grey">Lorem ipsum dolor sit amet consectetur</span></div>
                    <div class="text-footer"><h3><strong class="white">DC COMICS</strong></h3><br><span class="grey">Lorem ipsum dolor sit amet consectetur</span></div>
                    <div class="text-footer"><h3><strong class="white">DC COMICS</strong></h3><br><span class="grey">Lorem ipsum dolor sit amet consectetur</span></div>
                </div>
                <div class="footer__dx"></div>
            </div>
        </div>
        <div class="footer__bottom">
            <div class="footer__container-1">

                <h3 class="sign-up white">SIGN UP NOW!</h3>

                <div class="follow-us"></div>
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

    &__container {
        margin: auto;
        width: var(--container-md);

        @include listInline;
    }

    &__container-1 {
        margin: auto;
        width: var(--container-md);
        align-items: center;
        @include listInline;
        height: 120px;
        
    }

    &__top {
        width: 100vw;
        height: 150px;
        background-color: var(--primary-color);
        @include listInline;
        justify-content: space-between;

        img {
            max-width: 100%;
            max-height: 100%;
            margin: auto;
            padding: 50px;
        }
        
    }

    &__mid {
        @include listInline;
        background-image: url(../assets/img/footer-bg.jpg);
        height: 300px;
        margin: auto;
    }

    &__sx {
        height: 100px;
        width: 35%;
        @include listInline;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    &__dx {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-position: center;
        background-repeat: no-repeat;
        height: 300px;
        width: 65%;
    }

    p {
        color: var(--white);
        margin-top: 65px;
    }  

    .text-footer {
        width: 30%;
        padding: 10px;
        margin-top: 10px;
    }

    &__bottom {
        background-color: var(--terzo-color);
        height: 120px;
    }

    .sign-up {
        border: 3px solid var(--primary-color);
        padding: 8px;
        
    }
}

</style>

