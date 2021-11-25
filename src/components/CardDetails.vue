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
 &__header{
    position: relative;
    display: flex;
    align-items: center;   
    padding: 24px;
    background-color: $color-extralightblue;
    box-shadow: 0px 0px 6px 0px $color-boxshadow;
    margin: 24px;
    border-radius: 8px;
    border: 1px solid $color-border;
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