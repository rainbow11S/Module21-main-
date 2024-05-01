<template>
  <div class="row air-block">
    <div class="block-1 col-lg-6 col-md-6">
      <h4 class="main-title">The air in the UAE</h4>
      <p class="text-block">
        The problem in Dubai is that oxygen concentrations are typically 10-20%
        below normal.
      </p>
    </div>
    <div class="block-2 col-lg-6 col-md-6">
      <h6 class="title-block">
        A 1.5% drop in oxygen means 7.5% more harmful gases like sulphur and
        nitrogen dioxide, leading to:
      </h6>
      <ul class="list-texts">
        <li class="list-text">Lower productivity.</li>
        <li class="list-text">Feelings of dizziness and fatigue.</li>
        <li class="list-text">Compromised immunity and metabolism.</li>
        <li class="list-text">Heart issues.</li>
        <li class="list-text">Respiratory ailments.</li>
      </ul>
    </div>
  </div>
</template>

<style scoped lang="scss">
.air-block {
  @include backImage("/images/air.png");
  @include sideIndents;

  flex-wrap: nowrap;
  min-height: 650px;
  border-radius: 30px;
  margin-top: 20px;
  padding: 40px;
  background-color: $gray;

  @include miniDesktop {
    min-height: 515px;
    padding: 30px;
    margin-top: 15px;
  }
  @include tablet {
    min-height: 420px;
  }
  @include invertTablet {
    min-height: 460px;
    padding: 25px;
    margin-top: 10px;
    flex-wrap: wrap;
    flex-direction: column;
  }
  @include invertPhone {
    min-height: 400px;
    padding: 20px;
    margin-top: 10px;
  }
  .block-1 {
    .main-title {
      @include blockHeadline;
    }
    .text-block {
      max-width: 445px;
      padding-top: 20px;

      @include miniDesktop {
        max-width: 360px;
        padding-top: 15px;
      }
      @include tablet {
        max-width: 330px;
      }
      @include invertTablet {
        max-width: 305px;
      }
      @include invertPhone {
        max-width: 295px;
        padding-top: 13px;
      }
    }
  }
  .text-block,
  .title-block,
  .list-text {
    @include miniText;
  }
  .block-2 {
    padding: 65px 0 0 10px;

    @include miniDesktop {
      padding: 35px 0 0 8px;
    }
    @include tablet {
      padding: 31px 0 0 8px;
    }
    @include invertTablet {
      padding: 30px 0 0 0;
    }
    .title-block {
      max-width: 530px;

      @include miniDesktop {
        max-width: 425px;
      }
      @include tablet {
        max-width: 340px;
      }
      @include invertTablet {
        max-width: 310px;
      }
      @include invertPhone {
        max-width: 290px;
      }
      @include phone {
        max-width: 240px;
      }
    }
    .list-texts {
      padding: 15px 0 0 12px;
      margin: 0;

      @include invertTablet {
        padding: 13px 0 0 12px;
      }
    }
  }
}
</style>
