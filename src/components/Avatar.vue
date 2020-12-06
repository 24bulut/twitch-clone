<template>
  <figure>
    <img
      :height="size"
      :width="size"
      alt="Kullanıcı Profil Resmi"
      :src="src"
    />
  </figure>
</template>

<script>
export default {
  props: {
    size: {
      type: String,
    },
    src: {
      type: String,
      default: "https://static-cdn.jtvnw.net/user-default-pictures-uv/dbdc9198-def8-11e9-8681-784f43822e80-profile_image-70x70.png"
    },
  },
};
</script>

<style lang="less" scoped>
img {
  border-radius: 100%;
}
</style>
