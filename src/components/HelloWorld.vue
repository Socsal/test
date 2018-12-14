<template>
  <div class="a">
    <select-item
      v-for="(item,index) in items"
      :key="index"
      :name="item.name"
      :count="item.count"
      :avator="item.avator"
      :support="item.support"
      :blage="item.blage"
      :blageImg="item.blageImg"
      :index="index"
    ></select-item>
  </div>
</template>

<script>
//引入
import SelectItem from "./SelectItem";
export default {
  components: { SelectItem },
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
  }
};
</script>
<style lang="less" scoped>
.a {
  display: flex;
  width: 100%;
  height: 150px;
  justify-content: space-between;
}
</style>


