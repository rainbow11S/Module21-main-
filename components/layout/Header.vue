<template>
  <header class="header-site">
    <NuxtLink>
      <img class="logo-site" src="/icons/module21-logo.svg" alt=""
    /></NuxtLink>
    <div class="links-site">
      <NuxtLink class="link">Cleaning process</NuxtLink>
      <NuxtLink class="link">Safe enrichment</NuxtLink>
      <NuxtLink class="link">Suitable for</NuxtLink>
    </div>
    <button class="button-form">I'm interested</button>
  </header>
</template>

<style scoped lang="scss">
.header-site {
  display: flex;
  justify-content: space-between;
  height: 28px;
  background-color: #1a1a1a;

  .logo-site {
    width: 169px;
    height: 16px;
    margin: 5px 0 7px 0;
  }
  .links-site {
    display: flex;
    gap: 0 30px;
    margin: 8px 0;

    .link {
      @include pitch;

      color: #ffffff;
      font-size: 12px;
      letter-spacing: -6.5%;
    }
  }
  .button-form {
    @include pitch;

    width: 128px;
    height: 28px;
    border: 0;
    border-radius: 100px;
    background-color: #ffffff;
    color: 141414;
    font-size: 12px;
    letter-spacing: -6.5%;
  }
}
</style>
