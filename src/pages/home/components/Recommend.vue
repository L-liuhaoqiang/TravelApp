<template>
    <div>
        <div class="recommend-title">热销推荐</div>
        <ul>
            <li class="item border-bottom" v-for="item of recommendList" :key="item.id" >
                    <img class="item-img" :src="item.imgUrl">
                <div class="item-info">
                    <p class="item-title">{{item.title}}</p>
                    <p class="item-desc">{{item.desc}}</p>
                    <button class="item-button">查看详情</button>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1606/74/74f937d6d4b0d4cb90.water.jpg_200x200_63a86b4c.jpg',
        title: '白鹿温泉加勒比水上乐园',
        desc: '白鹿温泉水上乐园是白鹿温泉的升级项目'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1606/74/74f937d6d4b0d4cb90.water.jpg_200x200_63a86b4c.jpg',
        title: '白鹿温泉加勒比水上乐园',
        desc: '白鹿温泉水上乐园是白鹿温泉的升级项目'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1606/74/74f937d6d4b0d4cb90.water.jpg_200x200_63a86b4c.jpg',
        title: '白鹿温泉加勒比水上乐园',
        desc: '白鹿温泉水上乐园是白鹿温泉的升级项目'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.recommend-title
    line-height:.8rem
    background:#ccc
    text-indent:.2rem
    margin-top:.2rem
.item
    display:flex
    height.1.9rem
    overflow:hidden
    .item-img
        width:1.7rem
        height:1.7rem
        padding:.1rem
    .item-info
        flex:1
        padding:.1rem
        min-width:0
        .item-title
            overflow:hidden
            white-space:nowrap
            text-overflow: ellipsis
            line-height:.54rem
            font-size:.32rem
        .item-desc
            line-height:.4rem
            color:#ccc
            overflow:hidden
            white-space:nowrap
            text-overflow: ellipsis
        .item-button
            line-height:.44rem
            margin-top:.16rem
            color:#fff
            background:#ff9300
            padding:0 .2rem
            border-radius:.06rem
</style>
