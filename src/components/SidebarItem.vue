<template> 
      <a class="sidebar-item">
        <Avatar
          :size="30"
          src="https://static-cdn.jtvnw.net/jtv_user_pictures/b8597053-45b2-4534-bc98-0ab0055a9a11-profile_image-70x70.png"
        />
        <div class="status-bar">
          <div class="status">
          <CustomText
            tag="p"
            class="nick-name"
            size="size-5"
            weight="weight-semibold"
          >
            XANTAREScN
          </CustomText>
          <CustomText
            tag="p"
            class="info"
            size="size-6"
            
          >
            Sadece Sohbet
          </CustomText>
          </div>
          <div class="live-status">
            <div class="record"></div>
            <CustomText tag="p" class="viewer" size="size-6">
              4,6 B
            </CustomText>
          </div>
        </div>
      </a>
</template>

<script>
import CustomText from "./CustomText";
import Avatar from "./Avatar.vue";

export default {
  components: {
    CustomText,
    Avatar
  }
};
</script>

<style lang="less" scoped>
@import "../styles/variables";
@import "../styles/theme-light";
.sidebar-item {
  cursor: pointer;
  height: 4.2rem !important;
  width: 100%;
  display: flex;
  align-items: center;
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  padding-right: 1rem;
  padding-left: 1rem;
  &:hover {
    background: #e6e6ea;
  }
  & > .status-bar {
    flex: 1;
    display: flex;
    justify-content: space-between;
    & > .status {
      margin-left: 1rem;
      & > .info {
        color: @color-text-alt-2!important;
      }
    }

    & > .live-status {
      display: flex;
      align-items: center;
      .record {
        width: 0.8rem;
        height: 0.8rem;
        background-color: red;
        border-radius: 100%;
      }
      .viewer {
        color: @color-text-alt-2!important;
        margin-left: 0.5rem;
      }
    }
  }
}
</style>
