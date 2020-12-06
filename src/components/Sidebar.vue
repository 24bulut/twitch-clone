<template>
  <div class="sidebar">
    <div class="sidebar-items">
      <div class="sidebar-header ">
        <CustomText tag="h6" size="size-6" weight="weight-semibold">
          TAKİP EDİLEN KANALLAR
        </CustomText>
        <ButtonIcon>
          <HideLayout width="2rem" height="2rem" fill="#000" />
        </ButtonIcon>
      </div>
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />
      <SidebarItem />

    </div>
    <div class="search-form">
      <Search class="icon" width="2rem" height="2rem" fill="#53535f" />
      <Input placeholder="Arkadaş Eklemek İçin Ara" />
    </div>
  </div>
</template>

<script>
import CustomText from "./CustomText";
import ButtonIcon from "./ButtonIcon";
import SidebarItem from "./SidebarItem";
import Input from "./Input";
import HideLayout from "../icons/HideLayout.svg";
import Search from "../icons/Search.svg";

export default {
  components: {
    CustomText,
    HideLayout,
    ButtonIcon,
    Input,
    Search,
    SidebarItem
  },
};
</script>

<style lang="less" scoped>
@import "../styles/variables";
@import "../styles/theme-light";

.sidebar {
  background-color: @color-background-alt;
  width: 240px;
  min-width: 240px;
  height: 100%;
  display: flex;
  flex-direction: column;
  .search-form {
    height: 50px;
    padding: 1rem;
    border-top: @border-width-default solid @color-border-base !important;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;

    & > input {
      width: 100%;
      padding-left: 3rem;
    }
    & > .icon {
      position: absolute;
      left: 1.7rem;
    }
  }
  .sidebar-items {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    overflow:auto;

    .sidebar-header {
      display: flex;
      padding: 1.1rem;
      justify-content: space-between;
      align-items: center;
      width: 100%;
    }
  }
}
</style>
