<template>
  <main class="main">
      <div class="main__text">
          <h2> Content goes here </h2>
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
    background-color: var(--secondary-color);
    height: 9.375rem;
    align-items: center;

    h2 {
        color: var(--white);
    }
}

</style>