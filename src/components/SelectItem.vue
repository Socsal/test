<template>
  <div class="select-item">
    <!-- {{name}} -->
    <div class="item">
      <div>
        <div>
          <img :src="avator" alt="头像" class="avator">
        </div>

        <div v-if="blage == 'img'" class="blage">
          <img :src="blageImg" class="blageImg">
        </div>
        <div v-else class="blage">
          <div class="blageText">{{index+1}}</div>
        </div>

        <div class="message">
          <div class="name">{{name}}</div>
          <div class="count">{{count}}</div>
          <div class="support">{{support}}</div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    name: {
      type: String,
      default: "aaa"
    },
    count: {
      type: String,
      default: "aaa"
    },
    support: {
      type: String,
      default: "aaa"
    },
    avator: {
      type: String,
      default: null
    },
    blageImg: {
      type: String,
      default: null
    },
    blage: {
      type: String,
      default: null
    },
    index: {
      type: String,
      default: null
    }
  }
};
</script>
<style lang="less" scoped>
.item {
  width: 75px;
  height: 150px;
  display: flex;
  flex-direction: column;
  align-items: center;

  .avator {
    width: 64px;
    height: 64px;
    border-radius: 50px;
    background: yellow;
  }

  .blage {
    margin-top: -15px;
    // background: red;
    display: flex;
    justify-content: center;
    align-items: center;

    .blageImg {
      width: 20px;
      height: 20px;
      background: rgba(128, 128, 128, 0.8);
      border-radius: 50px;
    }
    .blageText {
      width: 40px;
      height: 20px;
      background: rgba(128, 128, 128, 0.8);
      color: white;
      border-radius: 50px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 12px;
    }
  }

  .message {
    .name {
      font-weight: bold;
    }
    .count {
      color: red;
      font-size: small;
    }
    .support {
      color: gray;
      font-size: small;
    }
  }
}
</style>
