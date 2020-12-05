<template>
  <a class="nav-link link">
    <CustomText tag="p" size="size-5" weight="weight-semibold"
      ><slot
    /></CustomText>
  </a>
</template>

<script>
import CustomText from "./CustomText";
export default {
  name: "NavLink",
  components: {
    CustomText,
  },
};
</script>

<style lang="less" scope>
.nav-link {
  display: flex;
  align-items: center;
  cursor: pointer;
  & > p {
    padding-right: 1rem;
    padding-left: 1rem;
  }
}
.active{
  border-bottom: 2px solid #772ce8;
}
</style>
