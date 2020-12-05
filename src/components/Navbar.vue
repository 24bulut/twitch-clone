<template>
  <nav class="navbar">
    <div class="firstbar">
      <div class="logo">
        <Logo />
      </div>
      <div class="nav">
        <NavLink>Takip Edilen</NavLink>
        <NavLink>Gözat</NavLink>
      </div>
        <div>
          <ButtonIcon>
            <MoreIcon width="2rem" height="2rem" fill="#000" />
          </ButtonIcon>
        </div>
      
    </div>
    <div class="secondbar">
      <SearchBar/>
    </div>
    <div class="Thirdbar"></div>
  </nav>
</template>

<script>
import Logo from "./Logo";
import NavLink from "./NavLink";
import ButtonIcon from "./ButtonIcon";
import MoreIcon from "../icons/More.svg";
import SearchBar from './SearchBar.vue';

export default {
  name: "Navbar",
  components: {
    Logo,
    MoreIcon,
    NavLink,
    SearchBar,
    ButtonIcon
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
  border-bottom: 1px solid #ddd;
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
  .secondbar{
    padding-left: 2rem;
    padding-right: 2rem;

  }
}
</style>
