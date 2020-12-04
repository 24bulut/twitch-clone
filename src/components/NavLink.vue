<template>
  <div class="nav-link">
    <CustomText tag="p" size="size-5" weight="weight-semibold"
      ><slot
    /></CustomText>
  </div>
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
  & > p {
    padding-right: 1rem;
    padding-left: 1rem;
  }
}
</style>
