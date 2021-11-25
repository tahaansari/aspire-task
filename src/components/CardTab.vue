<template>
    <div class="card-tab">
        <div class="card-tab__item">
            <a href="#" class="card-tab__anchor card-tab__anchor--active">My debit cards</a>
        </div>
        <div class="card-tab__item">
            <a href="#" class="card-tab__anchor">All company cards</a>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.card-tab{
    display: flex;
    font-size: 1.3rem;
    &__item{
        padding-right: 33px;
    }
    &__anchor{
        display: inline-block;
        padding-bottom: 2px;
        opacity: .5;
    }
    &__anchor--active{
        opacity: 1;
        border-bottom: 2px solid $color-skyblue;
    }
}
</style>