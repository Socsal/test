<template>
  <div class="common-item">
    <div class="item">
      <div class="cover">
        <img :src="cover" alt="封面" class="cover">
        <div class="info">
          <div>播放{{playCount}}</div>
          <div>弹幕{{dmkCount}}</div>
          <div>时长{{Duration}}</div>
        </div>
      </div>
      <div class="title">{{title}}</div>
      <div class="other">
        <div class="part">{{part}}</div>
        <button class="option"></button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    cover: {
      type: String,
      default: null
    },
    playCount: {
      type: String,
      default: null
    },
    dmkCount: {
      type: String,
      default: null
    },
    Duration: {
      type: String,
      default: null
    },
    title: {
      type: String,
      default: null
    },
    part: {
      type: String,
      default: null
    }
  }
};
</script>

<style lang="less" scoped>
.common-item {
  width: 49%;
  .item {
    background: white;
    // width: 100%;
    border-radius: 10px;
    margin-top: 8px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;

    .cover {
      border-radius: 10px;

      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;

      .info {
        width: 100%;
        background: rgba(128, 128, 128, 0.6);
        border-bottom-left-radius: 10px;
        border-bottom-right-radius: 10px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 10px;
        margin-top: -15px;
        color: rgba(255, 255, 255, 0.9);
      }
    }
    .title {
      height: 40px;
      text-align: left;
      overflow: hidden;
      font-size: 14px;
    }

    .other {
      width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: nowrap;
      flex-direction: row;

      .part {
        margin-left: 5px;
        font-size: 10px;
        color: gray;
      }
      .option {
        height: 10px;
        margin-right: 5px;
        border: none;
        color: white;
        background-color: gray;
      }
    }
  }
}
</style>

