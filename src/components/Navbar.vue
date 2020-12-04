<template>
  <nav class="navbar">
    <div class="firstbar">
      <div class="logo">
        <Logo />
      </div>
      <div class="nav">
        <NavLink>Takip Edilenler</NavLink>
        <NavLink>Gözat</NavLink>
      </div>
        <div>
          <button class="button-icon">
            <MoreIcon width="2rem" height="2rem" fill="#000" />
          </button>
        </div>
      
    </div>
    <div class="secondbar"></div>
    <div class="Thirdbar"></div>
  </nav>
</template>

<script>
import Logo from "./Logo";
import NavLink from "./NavLink";

import MoreIcon from "../icons/More.svg";

export default {
  name: "Navbar",
  components: {
    Logo,
    MoreIcon,
    NavLink,
  },
};
</script>

<style lang="less" scoped>
@import "../styles/variables";

.navbar {
  height: 50px;
  width: 100%;
  background-color: white;
  display: flex;
  & > div {
    flex: 1;
    display: flex;
  }
  .nav{
      display: flex;
  }

  .firstbar {
    justify-content: start;
    align-items: center;
    .logo {
      padding: 0.5rem;
    }
  }
}
</style>
