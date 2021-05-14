<template>
  <view>
			<view class="topbanner">
				<view class="header">
					<view class="logo">
						<image src="../../static/img/logo.png" mode=""></image>
					</view>
					<view class="search">
						<image src="../../static/img/search.png"></image>
						<text>搜索商品名称</text>
					</view>
					<view class="user">
						<image src="../../static/icon/user.png" mode=""></image>
					</view>
				</view>
				<view class="nav">
				<ul>
					<li>
						<text :class="{ active: navIndex === -1 }" @click="changeNav(-1)"
							>推荐</text
						>
					</li>
					<li
						v-for="(item, index) in navItems"
						:key="index"
						@click="changeNav(index)"
					>
						<text :class="{ active: navIndex === index }">{{ item }}</text>
					</li>
				</ul>
			</view>
		</view>
		<view class="recom">
			<transition>
				<Recommend v-if="cateListIndex ===-1"></Recommend>
				<Shouji v-if="cateListIndex ===0"></Shouji>
				<Zhineng v-if="cateListIndex ===1"></Zhineng>
				<Dianshi v-if="cateListIndex ===2"></Dianshi>
				<Jiadian v-if="cateListIndex ===3"></Jiadian>
				<Bijiben v-if="cateListIndex ===4"></Bijiben>
			</transition>
		</view>
  </view>
</template>

<script>
import Recommend from "../recommend/recommend.vue";
import Bijiben from '../cateLists/bijiben/bijiben.vue';
import Dianshi from '../cateLists/dianshi/dianshi.vue';
import Shouji from '../cateLists/shouji/shouji.vue';
import Jiadian from '../cateLists/jiadian/jiadian.vue';
import Zhineng from '../cateLists/zhineng/zhineng.vue';
export default {
  components: {
    Recommend,
    Bijiben,
    Dianshi,
    Zhineng,
    Jiadian,
    Shouji
  },
  data() {
    return {
      navItems: ["手机", "智能", "电视", "家电", "笔记本"],
      navIndex: -1,
			cateListIndex:-1
    };
  },
  methods: {
    changeNav(index) {
      this.navIndex = index;
			this.cateListIndex = index
    },
  },
};
</script>

<style lang="less">
	.topbanner{
		background-color: #f2f2f2;
		top: 0;
		left: 0;
		position: fixed;
		width: 100%;
		height: 73.76*2rpx;
		z-index: 1;
	}
.recom{
	margin-top: 73.76*2rpx;
}
* {
  margin: 0;
  padding: 0;
}
.nav {
  width: 100%;
  background-color: #f2f2f2;
  ul {
    display: flex;
    width: 100%;
    height: 60rpx;
    li {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-grow: 1;
      list-style: none;
      text {
        color: #747474;
        box-sizing: border-box;
        line-height: 60rpx;
        font-size: 28rpx;
        height: 60rpx;
      }
      .active {
        color: #ff6700;
        border-bottom: 2px solid #ff6700;
      }
    }
  }
}
.header {
  width: 100%;
  height: 43.76 * 2rpx;
  display: flex;
  align-items: center;
  background-color: #f2f2f2;

  .logo {
    display: flex;
    height: 100%;
    width: 52.09 * 2rpx;
    justify-content: center;
    align-items: center;

    image {
      width: 25 * 2rpx;
      height: 16.44 * 2rpx;
    }
  }
  .user {
    width: 52.09 * 2rpx;
    height: 31.26 * 2rpx;
    display: flex;
    justify-content: center;
    align-items: center;
    image {
      width: 20 * 2rpx;
      height: 20 * 2rpx;
    }
  }
  .search {
    border-radius: 4rpx;
    flex-grow: 1;
    height: 33.26 * 2rpx;
    background-color: #ffffff;
    display: flex;
    color: #b2b2b2;
    align-items: center;
    image {
      margin: 0 10rpx;
      width: 20 * 2rpx;
      height: 20 * 2rpx;
    }
  }
}
</style>
