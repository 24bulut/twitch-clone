<template>
  <nav class="navbar">
    <div class="firstbar">
      <div class="logo">
        <Logo />
      </div>
      <div class="nav-link">
        <div>
          <CustomText tag="p" size="size-5" weight="weight-semibold"
            >Takip Edilen</CustomText
          >
        </div>
        <div>
          <CustomText tag="p" size="size-5" weight="weight-semibold"
            >Gözat</CustomText
          >
        </div>
        <div>
            <button>
                <MoreIcon width="2rem" height="2rem"  fill="#000"/>
            </button>
        </div>
      </div>
    </div>
    <div class="secondbar"></div>
    <div class="Thirdbar"></div>
  </nav>
</template>

<script>
import Logo from "./Logo";
import CustomText from "./CustomText";
import MoreIcon from "../icons/More.svg";

export default {
  name: "Navbar",
  components: {
    Logo,
    CustomText,
    MoreIcon,
  },
};
</script>

<style lang="less" scoped>
@import "../styles/variables";

.navbar {
  height: 50px;
  width: 100%;
  background-color: aqua;
  display: flex;
  & > div {
    flex: 1;
    display: flex;
  }
  .nav-link {
    display: flex;
    align-items: center;
    & > div {
      padding-right: 1rem;
      padding-left: 1rem;
    }
  }
  .firstbar {
    justify-content: start;
    .logo {
      padding: 0.5rem;
    }
  }
}
</style>
