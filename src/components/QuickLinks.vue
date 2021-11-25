<template>
  <div class="quick-links">
      <div class="quick-links__item">
          <a class="quick-links__icon quick-links__icon--freezecard" href="#">
              Freeze card
          </a>
      </div>
      <div class="quick-links__item">
          <a class="quick-links__icon quick-links__icon--setspendlimit" href="#">
              Set spend limit
          </a>
      </div>
      <div class="quick-links__item">
          <a class="quick-links__icon quick-links__icon--addtogpay" href="#">
              Add to GPay
          </a>
      </div>
      <div class="quick-links__item">
          <a class="quick-links__icon quick-links__icon--replacecard" href="#">
              Replace card
          </a>
      </div>
      <div class="quick-links__item">
          <a class="quick-links__icon quick-links__icon--cancelcard" href="#">
              Cancel card
          </a>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.quick-links{
    display: flex;
    justify-content: space-around;
    background-color: $color-lightblue;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
    padding: 20px 27px;
    @media (min-width: $md) {
        margin: 0 24px;
        border-radius: 15px;
    }
    &__item{
        padding: 0 5px;
    }
    &__icon{
        display: inline-block;
        padding-top: 40px;
        text-align: center;
        line-height: 1.4;
        font-size: 1.3rem;
        color: $color-darkestblue;
    }
    &__icon--freezecard{
        background: url(../assets/images/icons/freeze-card.svg) no-repeat top;
    }
    &__icon--setspendlimit{
        background: url(../assets/images/icons/set-spend-limit.svg) no-repeat top;
    }
    &__icon--addtogpay{
        background: url(../assets/images/icons/add-to-gpay.svg) no-repeat top;
    }
    &__icon--replacecard{
        background: url(../assets/images/icons/replace-card.svg) no-repeat top;
    }
    &__icon--cancelcard{
        background: url(../assets/images/icons/cancel-card.svg) no-repeat top;
    }
}
</style>