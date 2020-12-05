<template>
  <nav class="navbar">
    <div class="firstbar">
      <div class="logo">
        <Logo />
      </div>
      <div class="nav">
        <NavLink class="active">Takip Edilen</NavLink>
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
    <div class="thirdbar">
        <ButtonIcon>
          <King width="2rem" height="2rem" fill="#000" />
        </ButtonIcon>
        <ButtonIcon>
          <Notification width="2rem" height="2rem" fill="#000" />
        </ButtonIcon>
        <ButtonIcon>
          <Message width="2rem" height="2rem" fill="#000" />
        </ButtonIcon>
        <Button>
          <Bit width="2rem" height="2rem" fill="#000" />Bit Al
        </Button>
        <Avatar size="30px"/>
       
    </div>
  </nav>
</template>

<script>
import Logo from "./Logo";
import NavLink from "./NavLink";
import ButtonIcon from "./ButtonIcon";
import Button from "./Button";
import Avatar from "./Avatar";
import MoreIcon from "../icons/More.svg";
import King from "../icons/King.svg";
import SearchBar from './SearchBar.vue';
import Message from "../icons/Message.svg";
import Notification from "../icons/Notification.svg";
import Bit from "../icons/Bit.svg";



export default {
  name: "Navbar",
  components: {
    Logo,
    MoreIcon,
    NavLink,
    SearchBar,
    King,
    ButtonIcon,
    Message,
    Notification,
    Button,
    Bit,
    Avatar
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
      height: 100%;
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
  .thirdbar{
    justify-content: flex-end;
    align-items: center;
    padding-right: 1rem;
    & >  button{
      margin-left: .5rem;
      margin-right: .5rem;
    }
  }
}
</style>
