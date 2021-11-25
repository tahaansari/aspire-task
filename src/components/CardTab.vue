<template>
    <div class="card-tab">
        <div class="card-tab__item">
            <a href="#" class="card-tab__anchor" v-bind:class="{ 'card-tab__anchor--active' : selected == 1}" v-on:click="selected = 1">My debit cards</a>
        </div>
        <div class="card-tab__item">
            <a href="#" class="card-tab__anchor" v-bind:class="{ 'card-tab__anchor--active' : selected == 2}" v-on:click="selected = 2">All company cards</a>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            selected:1
        }
    },

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
        font-weight: 700;
    }
}
</style>