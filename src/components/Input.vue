<template>
  <input type="text" class="input" name="" id="" v-model="search" @input="handleButtonEnable" :placeholder="placeholder" />
</template>

<script>
export default {
    props:{
        placeholder:{
            type: String
        }
    },
    methods:{
        handleButtonEnable(e){
            this.$emit("handle:buttonEnable",e);
        }
    }
}
</script>

<style lang="less" scoped>
@import "../styles/variables";
@import "../styles/theme-light";

.input{
    -moz-appearance: none;
    -webkit-appearance: none;
    appearance: none;
    border: @border-width-input solid @color-border-input;
    color: @color-text-input;
    height: 3rem;
    line-height: 1.5;
    transition: box-shadow .1s ease-in,border .1s ease-in,background-color .1s ease-in;
    background-color: @color-background-input;
    background-clip: padding-box;
    padding-bottom: .5rem;
    padding-top: .5rem;
    padding-left: 1rem;
    padding-left: 1rem;
    border-radius: @border-radius-medium;
    font-size: @font-size-6!important;
}
.input:hover{
    border-color: @color-border-input-hover;
    outline: 0;
    background-color: @color-background-input;
}
.input:focus{
    background-color: @color-background-input-focus;
    border: @border-width-input solid @color-border-input-focus;
    outline: 0;
}
        
</style>
