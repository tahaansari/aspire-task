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
  color:$color-white;
  padding:24px;
  padding-top: 40px;
  padding-bottom: 40px;
  @media (min-width: $md) {
      position: static;
      background-color: $color-white;
      color:$color-black;
      padding-bottom: 20px;
  }
  &__header{
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      margin-bottom: 20px;
  }
}
</style>