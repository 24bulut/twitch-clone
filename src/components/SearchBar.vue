<template>
  <div class="search-bar">
      <Input   placeholder="Ara" />
      <Button class="button-disabled"><Search/></Button>
  </div>
</template>

<script>
import Button from './Button.vue';
import Input from "./Input";
import Search from "../icons/Search.svg";


export default {
  name: "SearchBar",
  methods:{
    deneme:function(){
      alert("deneme çalıştı !");
    }
  },
  components:{
    Input,
    Button,
    Search
  }
}
</script>

<style lang="less" scoped>
@import "../styles/variables";
@import "../styles/theme-light";
.search-bar{
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    .input{
        max-width: 350px;
        width: 100%;
        padding: 1.6rem;
        border-top-right-radius: 0px;
        border-bottom-right-radius: 0px;

    }
    button{
        width: 35px;
        height: @button-size-large;
        border-top-left-radius: 0px;
        border-bottom-left-radius: 0px;

    }
    

}

</style>