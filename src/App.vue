<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
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
.root{
  display: flex;
}
main{
  padding: 3rem;
  flex:1;
}
</style>
