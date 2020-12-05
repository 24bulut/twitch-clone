<template>
  <div class="sidebar">
      <div class="sidebar-header">
            <CustomText   tag="h6" size="size-6" weight="weight-semibold">
                  TAKİP EDİLEN KANALLAR
            </CustomText>
            <ButtonIcon>
                <HideLayout width="2rem" height="2rem" fill="#000" />
            </ButtonIcon>
      </div>
      <div class="search-form">

      </div>
  </div>
</template>

<script>
import CustomText from "@/components/CustomText";
import ButtonIcon from "@/components/ButtonIcon";
import HideLayout from "../icons/HideLayout.svg";

export default {
    components:{
        CustomText,
        HideLayout,
        ButtonIcon
    }

}
</script>

<style lang="less" scoped>
.sidebar{
    width: 240px;
    min-width: 240px;
    .sidebar-header{
        display: flex;
        padding: 1.1rem;
        justify-content: space-between;
        align-items: center;
    }
}
</style>