<template>
  <div class="a">
    <div v-for="(item,num) in sortItems" class="item" :key="num">
      <div>
        <img :src="item.icon" alt="头像" class="icon">
      </div>

      <div class="num">
        <div v-if="num+1==1">
          <img :src="icon_1" alt="第一" class="icon">
        </div>
        <div v-else-if="num+1==2">
          <img :src="icon_2" alt="第二" class="icon">
        </div>
        <div v-else-if="num+1==3">
          <img :src="icon_3" alt="第三" class="icon">
        </div>
        <div v-else class="icon2">{{num+1}}</div>
      </div>

      <div class="message">
        <div class="name">{{item.name}}</div>
        <div class="count">{{item.count}}</div>
        <div class="support">{{item.support}}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      icon_1: require("../assets/1.png"),
      icon_2: require("../assets/2.png"),
      icon_3: require("../assets/3.png"),
      items: [
        {
          name: "Martin",
          count: 245675,
          icon:
            "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=300533062,3547534330&fm=27&gp=0.jpg",
          num: 1,
          support: "support"
        },
        {
          name: "VXX",
          count: 145675,
          icon:
            "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=2403459980,910700322&fm=27&gp=0.jpg",
          num: "2",
          support: "support"
        },
        {
          name: "CXC",
          count: 35675,
          icon:
            "https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1401043180,3347050769&fm=27&gp=0.jpg",
          num: "3",
          support: "support"
        },
        {
          name: "DTE",
          count: 675,
          icon:
            "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=904569741,1186006061&fm=27&gp=0.jpg",
          num: "4",
          support: "support"
        }
      ]
    };
  },

  computed: {
    sortItems: function() {
      return sortByKey(this.items, "count").reverse();
    }
  }
};
function sortByKey(array, key) {
  return array.sort(function(a, b) {
    var x = a[key];
    var y = b[key];
    return x < y ? -1 : x > y ? 1 : 0;
  });
}
</script>
<style lang="less" scoped>
.a {
  display: flex;
  width: 100%;
  height: 150px;
  justify-content: space-between;
  .item {
    width: 75px;
    height: 150px;
    display: flex;
    flex-direction: column;
    align-items: center;

    .icon {
      width: 64px;
      height: 64px;
      border-radius: 50px;
      background: yellow;
    }
  }
  .num {
    margin-top: -10px;
    // background: red;
    .icon {
      width: 20px;
      height: 20px;
      background: rgba(128, 128, 128, 0.7);
      border-radius: 50px;
    }
    .icon2 {
      width: 40px;
      height: 20px;
      background: rgba(128, 128, 128, 0.7);
      color: white;
      border-radius: 50px;
      margin-bottom: 4px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 12px;
    }
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
</style>


