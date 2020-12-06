<template>
  <div id="app">

    <Navbar />
    <div class="root">
      <Sidebar />
      <main>
        <router-view />
      </main>
    </div>

    
  </div>
</template>


<script>
import Navbar from "@/components/Navbar";
import Sidebar from "@/components/Sidebar";


export default {
    name:"App",
    components:{
        Navbar,
        Sidebar
    }

}
</script>

<style lang="less">
@import "./styles/variables";
.root{
  display: flex;
  height: @root-height;

}
main{
  overflow: auto;
  padding: 3rem;
  flex:1;
}
</style>
