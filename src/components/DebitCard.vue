<template>
    <div class="debit-card">
        <a href="#" class="debit-card__showcardnumber">Show card number</a>
        <div class="debit-card__content">
            <img class="debit-card__logo" src="@/assets/images/icons/logo.svg" alt="">
            <h2 class="debit-card__name">Mark Henry</h2>
            <div class="debit-card__number">
                <span class="debit-card__digit">* * * *</span>
                <span class="debit-card__digit">* * * *</span>
                <span class="debit-card__digit">* * * *</span>
                <span class="debit-card__digit">2020</span>
            </div>
            <div class="debit-card__details">
                <span class="debit-card__date">Thru: 12/20</span>
                <span class="debit-card__cvv">CVV: * * *</span>
            </div>
            <img class="debit-card__visalogo" src="@/assets/images/icons/visa-logo.svg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.debit-card{
    position: relative;
    @media (min-width: $md) {
        max-width: 50%;
    }
    &__showcardnumber{
        position: absolute;
        top:0;
        right: 0;
        transform: translateY(-100%);
        background-color: $color-white;
        color:$color-green;
        padding: 4px;
        padding-right: 10px;
        padding-left: 26px;
        border-top-left-radius:6px;
        border-top-right-radius:6px;
        font-size: 1.2rem;
        &:before{
            content: "";
            width: 16px;
            height: 16px;
            position: absolute;
            left: 6px;
            top: 50%;
            transform: translateY(-50%);
            background: url(../assets/images/icons/eye.svg) no-repeat center;
        }
        &:after{
            content: "";
            width: 10px;
            height: 10px;
            background-color: $color-white;
            position: absolute;
            right: 0;
            top: 100%;
        }
    }
    &__content{
        position: relative;
        padding: 24px;
        background-color: $color-green;
        border-radius: 12px;
        margin-top: 54px;
        font-weight: 700;
        @media (min-width: $md) {
            color:$color-white;
        }
    }
    &__logo{
        margin-bottom: 20px;
        display: block;
        margin-left: auto;
    }
    &__visalogo{
        display: block;
        margin-left: auto;
    }
    &__name{
        font-size: 2.2rem;
    }
    &__number{
        margin-top: 10px;
        margin-bottom: 10px;
    }
    &__digit{
        margin-right: 24px;
    }
    &__details{
        font-size: 1.3rem;
    }
    &__date{
        margin-right: 30px;
    }
}
</style>