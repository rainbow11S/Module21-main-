<!-- TODO -->
1. Сделать миксины для падингов, шрифтов, цвета, заголовков, текста,
background-image 2. Play-image, play-button - переделать 3.

<template>
  <div class="description-block">
    <h1 class="main-title">MODULE 21</h1>
    <p class="text-block">Elevate your living with oxygen-enriched air.</p>
    <div class="description-advantages">
      <h6 class="description">
        Revitalize your day with the pioneering O2-enhancing air purifier.
      </h6>
      <div class="block-advantages">
        <div class="block-adv">
          <i class="number">1</i>
          <p class="advantage">A unique, one-of-a-kind machine.</p>
        </div>
        <div class="block-adv">
          <i class="number">2</i>
          <p class="advantage">Easy to install and operate.</p>
        </div>
        <div class="block-adv">
          <i class="number">3</i>
          <p class="advantage">Equipped with a remote control.</p>
        </div>
        <div class="block-adv">
          <i class="number">4</i>
          <p class="advantage">Improved well-being and quality of life.</p>
        </div>
        <button class="btn-interested">I'm interested</button>
      </div>
    </div>
    <div class="showreel">
      <img class="play-image" src="/images/play-image.png" alt="" />
      <button class="play-button">
        <img class="treyg-icon" src="/icons/treygolnik.svg" alt="" />
        <p class="play-text">Play showreel</p>
      </button>
    </div>
  </div>
</template>

<style scoped lang="scss">
.description-block {
  @include backImage("/images/module21-block.png");
  background-color: $gray;

  position: relative;
  padding: 20px;
  min-height: 910px;
  border-radius: 0 0 20px 20px;

  @include miniDesktop {
    min-height: 720px;
  }
  @include tablet {
    min-height: 720px;
  }
  @include invertTablet {
    min-height: 852px;
  }
  @include invertPhone {
    min-height: 640px;
  }
  @include phone {
    min-height: 700px;
    padding: 15px;
  }
  .main-title {
    @include conquera;
    color: $white;

    margin: 0;
    padding-top: 50px;
    font-size: 70px;

    @include miniDesktop {
      padding-top: 40px;
      font-size: 55px;
    }
    @include tablet {
      padding-top: 40px;
      font-size: 45px;
    }
    @include invertTablet {
      padding-top: 40px;
      font-size: 35px;
    }
    @include invertPhone {
      padding-top: 67px;
      font-size: 30px;
    }
    @include phone {
      padding-top: 72px;
      font-size: 25px;
    }
  }
  .text-block {
    @include pitch;

    color: #ffffff;
    font-size: 18px;
    padding-top: 20px;
    margin: 0;

    @include miniDesktop {
      font-size: 14px;
      padding-top: 15px;
    }
    @include tablet {
      font-size: 14px;
      padding-top: 12px;
    }
    @include invertTablet {
      font-size: 13px;
      padding-top: 11px;
    }
    @include phone {
      line-height: 120%;
      letter-spacing: -0.07em;
    }
  }
  .description,
  .number,
  .advantage {
    @include miniText;
  }
  .description {
    max-width: 430px;

    @include miniDesktop {
      max-width: 345px;
    }
    @include invertTablet {
      max-width: 320px;
    }
    @include invertPhone {
      max-width: 260px;
    }
  }
  .description-advantages {
    position: absolute;
    top: 58%;
    left: calc(50% + 10px);

    @include miniDesktop {
      left: calc(50% + 8px);
      top: 50%;
    }
    @include invertTablet {
      left: 20px;
      top: 43.4%;
    }
    @include invertPhone {
      top: 47.8%;
    }
    @include phone {
      top: 52%;
      left: 15px;
    }
    .block-advantages {
      display: flex;
      flex-direction: column;
      padding-top: 30px;

      @include miniDesktop {
        padding-top: 20px;
      }
      @include invertTablet {
        padding-top: 18px;
      }
      .block-adv {
        display: flex;
        align-items: center;
        gap: 8px;

        @include miniDesktop {
          gap: 6px;
        }
        .number {
          @include border($white20, $radius: 100%);
          width: 23px;
          height: 23px;
          text-align: center;

          @include miniDesktop {
            width: 18px;
            height: 18px;
            font-size: 11px;
          }
          @include invertTablet {
            font-size: 10px;
          }
        }
      }
    }
    .btn-interested {
      @include button;
      margin-top: 40px;

      @include miniDesktop {
        margin-top: 30px;
      }
      @include invertTablet {
        margin-top: 27px;
      }
    }
  }
  .showreel {
    position: absolute;
    width: 400px;
    height: 260px;
    bottom: 20px;
    left: 20px;

    @include miniDesktop {
      width: 315px;
      height: 205px;
    }
    @include tablet {
      width: 252px;
      height: 164px;
    }
    @include invertTablet {
      width: 230px;
      height: 140px;
    }
    @include invertPhone {
      width: 172px;
      height: 105px;
    }
    @include phone {
      left: 15px;
      bottom: 15px;
    }
    .play-image {
      width: 100%;
      height: 100%;
      border-radius: 30px;
    }
    .play-button {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: transparent;
      width: 100%;
      border: 0;
      .treyg-icon {
        width: 30px;
        height: 30px;

        @include miniDesktop {
          width: 24px;
          height: 24px;
        }
        @include invertTablet {
          width: 20px;
          height: 20px;
        }
      }
      .play-text {
        @include miniText;
        margin: 20px 0 0 0;

        @include miniDesktop {
          margin: 15px 0 0 0;
        }
        @include invertTablet {
          margin: 13px 0 0 0;
        }
      }
    }
  }
}
</style>
