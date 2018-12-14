<template>
  <div class="a">
    <div v-for="(item,index) in sortItems" class="item" :key="index">
      <div>
        <div>
          <img :src="item.avator" alt="头像" class="avator">
        </div>

        <div v-if="item.blage == 'img'" class="blage">
          <img :src="item.blageImg" class="blageImg">
        </div>
        <div v-else class="blage">
          <div class="blageText">{{index+1}}</div>
        </div>

        <div class="message">
          <div class="name">{{item.name}}</div>
          <div class="count">{{item.count}}</div>
          <div class="support">{{item.support}}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          name: "Martin",
          count: 245675,
          avator:
            "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=300533062,3547534330&fm=27&gp=0.jpg",
          support: "support",
          blage: "img",
          blageImg: "https://img-blog.csdnimg.cn/20181211170156940.png"
        },
        {
          name: "VXX",
          count: 145675,
          avator:
            "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=2403459980,910700322&fm=27&gp=0.jpg",
          support: "support",
          blage: "img",
          blageImg: "https://img-blog.csdnimg.cn/20181212091816917.png"
        },
        {
          name: "CXC",
          count: 35675,
          avator:
            "https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1401043180,3347050769&fm=27&gp=0.jpg",
          support: "support",
          blage: "img",
          blageImg: "https://img-blog.csdnimg.cn/20181212091846201.png"
        },
        {
          name: "DTE",
          count: 675,
          avator:
            "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=904569741,1186006061&fm=27&gp=0.jpg",
          support: "support",
          blage: "text"
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
}
</style>


