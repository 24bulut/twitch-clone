<template>
    <component :is="tag" :class="[size,weight]"  >
        <slot />
    </component>
</template>

<script>
    export default {
        name:"CustomText",
        props:{
            tag:{
                type: String,
                default:"span"
            },
            size:{
                type: String,
                default:"size-base",
                validator: function (value) {
                    // The value must match one of these strings
                    return ['size-1', 'size-2', 'size-3', 'size-4', 'size-5', 'size-6', 'size-7', 'size-8', 'size-base'].indexOf(value) !== -1
                }
            },
            weight:{
                type: String,
                default:"weight-normal",
                validator: function (value) {
                    // The value must match one of these strings
                    return ['weight-bold', 'weight-hdr','weight-normal','weight-semibold'].indexOf(value) !== -1
                }
            }
        }
        
    }
</script>

<style lang="less" scoped>
@import "../styles/variables";
p,
h1,
h2,
h3,
h4,
h5,
h6,
span,
b {
  font-family: inherit;
}

.size-base{
    font-size: @font-size-base;
}
.size-1{
    font-size: @font-size-1;
}
.size-2{
    font-size: @font-size-2;
}
.size-3{
    font-size: @font-size-3;
}
.size-4{
    font-size: @font-size-4;
}
.size-5{
    font-size: @font-size-5;
}
.size-6{
    font-size: @font-size-6;
}
.size-7{
    font-size: @font-size-7;
}
.size-8{
    font-size: @font-size-8;
}

.weight-bold{
    font-weight: @font-weight-bold;
}
.weight-normal{
    font-weight: @font-weight-normal;
}
.weight-semibold{
    font-weight: @font-weight-semibold;
}
.weight-hdr{
    font-weight: @font-weight-hdr;
}



</style>