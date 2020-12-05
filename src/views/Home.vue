<template>
 <div>

    <Button >Deneme</Button>
    <Input placeholder="deneme"/>
  <CustomText tag="h1" weight="weight-semibold" size="size-1" >
      Deneme
  </CustomText>
  <CustomText tag="h1" weight="weight-bold" size="size-1" >
      Takip Edilen
  </CustomText>
  <CustomText tag="h1" weight="weight-normal"  size="size-1">
      Takip Edilen
  </CustomText>
    <CustomText tag="h1" size="size-5">
      Takip Edilen
  </CustomText>
    <CustomText tag="h2"  size="size-8">
      Takip Edilen
  </CustomText>
  
 </div>
</template>

<script>
import CustomText from "@/components/CustomText"
import Button from "@/components/Button"
import Input from "@/components/Input"


export default {
    name:"Home",
    components:{
        CustomText,
        Button,
        Input
    }
}
</script>

<style>

</style>