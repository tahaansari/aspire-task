<template>
    <div class="cards">
        <div class="cards__header">
            <account-balance/>
            <btn-add-card/>
        </div>
        <card-tab/>
    </div>
</template>

<script>
import AccountBalance from './AccountBalance.vue'
import BtnAddCard from './BtnAddCard.vue'
import CardTab from './CardTab.vue'
export default {
    components: {
        AccountBalance,
        BtnAddCard,
        CardTab
    }
}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.cards{
  position: fixed;
  width: 100%;
  height: 100%;
  background-color: $color-darkestblue;
  color:$color-white;
  padding:24px;
  padding-top: 40px;
  padding-bottom: 70px;
  @media (min-width: $md) {
      position: static;
      width: calc(100% - 400px);
      margin-left: 400px;
      background-color: $color-white;
      color:$color-black;
      padding-top: 40px;
      padding-bottom: 70px;
  }
  &__header{
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      margin-bottom: 20px;
  }
}
</style>