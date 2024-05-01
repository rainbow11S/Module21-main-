<template>
  <div class="one-only">
    <div class="main-block">
      <h4 class="main-headline">The one and only</h4>
      <p class="text-block">
        This one-of-a-kind device not only boosts oxygen but also purifies
        harmful gases, safeguarding your health.
      </p>
    </div>
    <img class="module-image d-none" src="/images/oneOnly-2.png" alt="" />
  </div>
</template>

<style scoped lang="scss">
.one-only {
  @include sideIndents;

  display: flex;
  justify-content: space-between;
  margin-top: 20px;
  gap: 20px;
  min-height: 650px;

  @include miniDesktop {
    min-height: 514px;
    margin-top: 15px;
    gap: 15px;
  }
  @include tablet {
    min-height: 420px;
  }
  @include invertTablet {
    min-height: 460px;
    margin-top: 10px;
  }
  @include invertPhone {
    min-height: 400px;
  }
  @include phone {
    min-height: 460px;
  }

  .main-block,
  .module-image {
    border-radius: 30px;
  }
  .main-block {
    @include backImage("/images/oneOnly.png");

    width: 100%;
    padding: 40px;
    background-color: $gray;

    @include miniDesktop {
      max-width: 775px;
      padding: 30px;
    }
    @include tablet {
      max-width: 615px;
    }
    @include invertTablet {
      max-width: 100%;
    }
    @include invertPhone {
      padding-top: 20px;
    }

    .main-headline {
      @include blockHeadline;
    }
    .text-block {
      @include miniText;

      max-width: 470px;
      padding-top: 20px;

      @include miniDesktop {
        max-width: 375px;
        padding-top: 15px;
      }
      @include tablet {
        max-width: 335px;
      }
      @include invertTablet {
        max-width: 295px;
        padding-top: 13px;
      }
      @include phone {
        max-width: 270px;
      }
    }
  }
  .module-image {
    width: 100%;
    max-width: 480px;

    @include miniDesktop {
      max-width: 380px;
    }
    @include tablet {
      max-width: 300px;
    }
  }
}
</style>
