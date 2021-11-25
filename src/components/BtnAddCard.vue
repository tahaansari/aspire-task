<template>
      <a href="#" class="btn-add-card">New card</a>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
.btn-add-card{
    position: relative;
    color: $color-skyblue;
    font-size: 1.3rem;
    padding-left: 20px;
    @media (min-width: $md) {
       padding: 8px 12px;
       padding-left: 27px;
       background-color: $color-darkblue; 
       color: $color-white;
    }
    &:before{
        content: "";
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        width: 16px;
        height: 16px;
        border-radius: 50%;
        background:url(../assets/images/icons/add.svg) no-repeat center;
        @media (min-width: $md) {
            left: 7px;
        }
    }
}
</style>