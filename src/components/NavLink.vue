<template>
  <router-link :to="to" class="nav-link link">
    <CustomText tag="p" size="size-5" weight="weight-semibold"
      ><slot
    /></CustomText>
  </router-link>
</template>

<script>
import CustomText from "./CustomText";
export default {
  name: "NavLink",
  components: {
    CustomText,
  },
  props:{
    to:{
      type:String
    }
  }
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
.router-link-exact-active{
  border-bottom: 2px solid #772ce8;
}
</style>
