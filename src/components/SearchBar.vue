<template>
  <div class="search-bar">
    <Input @handle:buttonEnable="enableSearchButton"  placeholder="Ara" />
    <Button :class="{'button-disabled':!buttonEnable}" ><Search height="100%" /></Button>
  </div>
</template>

<script>
import Button from "./Button.vue";
import Input from "./Input";
import Search from "../icons/Search.svg";


export default {
  name: "SearchBar",
  data() {
    return {
      buttonEnable: false
    };
  },
  components: {
    Input,
    Button,
    Search
  },
  updated: function () {
      console.log(this.buttonEnable);
  },
  methods: {
    enableSearchButton(e){
      if (e.target.value.length > 0) {
          this.buttonEnable=true;
      }else{
          this.buttonEnable=false;
      }
    }
  }
};
</script>

<style lang="less" scoped>
@import "../styles/variables";
@import "../styles/theme-light";
.search-bar {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  .input {
    max-width: 350px;
    width: 100%;
    padding: 1.6rem;
    border-top-right-radius: 0px;
    border-bottom-right-radius: 0px;
  }
  button {
    width: 35px;
    height: @button-size-large;
    border-top-left-radius: 0px;
    border-bottom-left-radius: 0px;
    padding: 0.5rem;

  }
}
</style>
