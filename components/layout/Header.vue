<template>
  <header class="header-site">
    <NuxtLink>
      <img class="logo-site" src="/icons/module21-logo.svg" alt=""
    /></NuxtLink>
    <div class="links-site d-none">
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
  position: fixed;
  z-index: 1;
  width: 100%;
  height: 35px;
  margin: 20px 0;
  padding: 0 20px;
  top: 0;

  @include miniDesktop {
    height: 28px;
  }
  @include tablet {
    height: 27px;
  }
  @include phone {
    padding: 0 15px;
  }
  .logo-site {
    width: 229px;
    height: 20px;
    margin: 7px 0 7.5px 0;

    @include miniDesktop {
      width: 194px;
      height: 18px;
      margin: 5px 0;
    }
    @include tablet {
      width: 169px;
      height: 16px;
      margin: 5px 0 7px 0;
    }
    @include invertTablet {
      width: 180px;
      height: 15px;
      margin: 5px 0 7px 0;
    }
    @include invertPhone {
      width: 160px;
      height: 15px;
    }
    @include phone {
      width: 135px;
      height: 13px;
      margin: 7px 0;
    }
  }
  .links-site {
    display: flex;
    gap: 0 40px;
    margin: 10px 0;

    @include miniDesktop {
      gap: 0 30px;
      margin: 8px 0;
    }
    .link {
      @include miniText;
    }
  }
  .d-none {
    @include invertTablet {
      display: none;
    }
  }
  .button-form {
    @include button;
  }
}
</style>
