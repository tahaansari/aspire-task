<template>
  <div class="card-details">
      <div class="card-details__header">
        <img class="card-details__icon" src="@/assets/images/icons/card-details.svg" alt="">
        Card Details
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.card-details{
  padding: 12px 24px;
 &__header{
    position: relative;
    display: flex;
    align-items: center;   
    padding: 24px;
    border-radius: 8px;
    background-color: $color-extralightblue;
    border: 1px solid $color-border;
    box-shadow: 0px 0px 6px 0px $color-boxshadow;
    &:before{
        content: "";
        position: absolute;
        top: 50%;
        right: 24px;
        transform: translateY(-50%);
        width: 20px;
        height: 20px;
        background: url(../assets/images/icons/down-arrow.svg) no-repeat center/contain;
    }
 }
 &__icon{
     margin-right: 12px;
 }  
}
</style>