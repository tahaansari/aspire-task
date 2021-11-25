<template>
    <div class="account-balance">
        <div>Account Balance</div>
        <div class="account-balance__amount">
            <span class="account-balance__currency">S$</span>
            3,000
        </div>
    </div> 
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.account-balance{
    &__amount{
        font-size: 2.4rem;
        display: flex;
        align-items: center;
        margin-top: 10px;
        font-weight: 700;
    }
    &__currency{
        background-color: $color-green;
        padding: 2px 15px;
        border-radius: 4px;
        font-size: 1.4rem;
        margin-right: 10px;
    }
}
</style>