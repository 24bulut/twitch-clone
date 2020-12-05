<template>
  <button class="button button-default" >
    <slot />
  </button>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
@import "../styles/variables";
@import "../styles/theme-light";

.button-default {
  background-color: @color-background-button-secondary-default;
  color: @color-text-button-secondary;
  border-radius: @border-radius-medium;
  padding: 0.5rem;
  cursor: pointer;
}
.button-default:hover {
  background-color: @color-background-button-secondary-hover;
  color: @color-text-button-secondary;
}
.button-disabled{
  color: @color-text-button-disabled !important;
  fill: @color-text-button-disabled !important;
  background-color: @color-background-button-disabled !important;
  cursor: not-allowed !important;
}
</style>
