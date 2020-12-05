<template>
    <button class="button button-icon ">
        <slot />
    </button>
</template>

<script>
export default {

}
</script>

<style lang="less" scoped>
@import "../styles/variables";
@import "../styles/theme-light";

.button-icon {
  -ms-user-select: none;
  -webkit-user-select: none;
  align-items: center;
  background-color: transparent;
  background-color: @color-background-button-text-default;
  border-radius: @border-radius-medium;
  color: @color-fill-button-icon;
  display: inline-flex;
  height: @button-size-default;
  justify-content: center;
  user-select: none;
  width: @button-size-default;
  cursor: pointer;

}

.button-icon:not(:disabled):hover {
  background-color: @color-background-button-text-hover;
  color: @color-fill-button-icon-hover;
}

</style>