<template>
  <div class="a">
    <CommonItem
      v-for="(item,index) in items"
      :key="index"
      :cover="item.cover"
      :playCount="item.playCount"
      :dmkCount="item.dmkCount"
      :Duration="item.Duration"
      :title="item.title"
      :part="item.part"
    ></CommonItem>
  </div>
</template>


<script>
import CommonItem from "./CommonItem";
export default {
  components: { CommonItem },
  data() {
    return {
      items: [
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/87bcd320e5b8cf35a103258aad58c96f6266f3b2.jpg@320w_200h.webp",
          playCount: 58654,
          dmkCount: 173,
          Duration: "8:10",
          title: "FATE系列爆燃混剪——穿越黑夜的希望！！！！",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/c55ce6302f7a6015bc240f51ab538000f60705c1.jpg@320w_200h.webp",
          playCount: 16238,
          dmkCount: 430,
          Duration: "8:10",
          title: "治愈心灵/燃爆经费！美与燃的巅峰结合！",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i1.hdslb.com/bfs/archive/4de32363796c5107c62656aa9bbf9d17bd612f24.jpg@320w_200h.webp",
          playCount: 36000,
          dmkCount: 177,
          Duration: "8:10",
          title:
            "地球联邦军宇宙舰队力量展示MAD×麦哲伦级战列舰、萨拉米斯级巡洋舰、哥伦布级运输舰",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i1.hdslb.com/bfs/archive/ae09e2318d84f9621c900443eb021d247f027ce1.jpg@320w_200h.webp",
          playCount: 5,
          dmkCount: 0,
          Duration: "8:10",
          title: "【东京喰种/炫酷/AMV】精品Instagram edit",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i0.hdslb.com/bfs/archive/0eada36da588dbf46edca1c64b849d27da0beed7.jpg@320w_200h.webp",
          playCount: 17,
          dmkCount: 0,
          Duration: "8:10",
          title: "生而为人，我很抱歉，但错的不是我，而是这个世界!!!",
          part: "MAD·AMV"
        },
        {
          cover:
            "http://i2.hdslb.com/bfs/archive/1ebaa0ea0d69a2f6f343dffd1244d88bb490df9e.jpg@320w_200h.webp",
          playCount: 25964,
          dmkCount: 125,
          Duration: "8:10",
          title:
            "【已授权】狐妖小红娘：淮竹虽为妾，霸业未有妻，这才是最感人的告白～",
          part: "MAD·AMV"
        }
      ]
    };
  }
};
</script>


<style lang="less" scoped>
.a {
  background: rgb(233, 233, 233);
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  flex-wrap: wrap;
}
</style>

