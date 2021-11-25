<template>
  <div class="recent-transaction">
      <div class="recent-transaction__header">
        <img class="recent-transaction__icon" src="@/assets/images/icons/recent-transaction.svg" alt="">
        Recent Transaction
      </div>
      <div class="recent-transaction__list">
        <transaction/>
        <transaction/>
        <transaction/>
      </div>
      <div class="recent-transaction__viewall">
        <a href="#">View all card transactions</a>
      </div>
  </div>
</template>

<script>
import Transaction from './Transaction.vue'
export default {
  components: { Transaction },

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.recent-transaction{
  padding: 12px 24px;
  &__list{
    border: 1px solid $color-border;
    border-top: 0;
    border-bottom-left-radius:8px;
    border-bottom-right-radius:8px;
    background-color:$color-white;
    margin-top: -8px;
    margin-bottom: -8px;
    padding-top:10px;
  }
  &__viewall{
    position: relative;
    padding: 16px;
    padding-top: 24px;
    border: 1px solid $color-greenborder;
    border-top: 0;
    background-color: $color-lightgreen;
    border-bottom-left-radius: 8px;
    border-bottom-right-radius: 8px;
    color:$color-green;
    text-align: center;
  }
 &__header{
    position: relative;
    display: flex;
    align-items: center;   
    padding: 24px;
    background-color: $color-extralightblue;
    box-shadow: 0px 0px 6px 0px $color-boxshadow;
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