<template>
  <div class="transaction">
      <div class="transaction__icon">
          <span class="transaction__ico transaction__ico--filestorage"></span>
      </div>
      <div class="transaction__details">
        Hamleys
        <br>
        <span class="transaction__date">20 May 2020</span>
        <br>
        <span class="transaction__info">Charged to debit card</span>
      </div>
      <div class="transaction__price">
        + S$ 150
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.transaction{
    display: flex;
    border-bottom: 1px solid $color-border;
    &:last-child{
        border-bottom: 0;
    }
    padding: 18px 0;
    margin: 0 24px;
    justify-content: space-around;
    &__ico{
        display: inline-block;
        width: 48px;
        height: 48px;
        border-radius: 50%;
    }
    &__ico--filestorage{
        background: $color-lightblue url(../assets/images/icons/file-storage.svg) no-repeat center;
    }
    &__date{
        display: inline-block;
        color: $color-lightgray;
        font-size: 1.3rem;
        line-height: 2;
    }
    &__details{
        padding: 0 12px;
    }
    &__info{
        display: inline-block;
        position: relative;
        padding-left: 28px;
        color: $color-darkblue;
        font-weight: 600;
        font-size: 1.2rem;
        line-height: 2.5;
        &:before{
            content: "";
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            left: 0;
            width: 24px;
            height: 20px;
            border-radius: 20px;
            background: $color-darkblue url(../assets/images/icons/business-and-finance.svg) no-repeat center;
        }
    }
    &__price{
        color: $color-green;
        font-weight: 700;
        flex:1;
        text-align: right;
    }
}
</style>