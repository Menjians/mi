<template>
	<view>
		<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000" indicator-active-color="#fff" indicator-color="#eee">
			<swiper-item>
				<view class="swiper-item">
					<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/0b2bb13c396cc6205dd91da3a91a275a.jpg?thumb=1&w=720&h=360" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">
					<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/37bd342303515c7a1a54681599e319a1.jpg?thumb=1&w=720&h=360" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">
					<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/bb4a8b7d9e77567c7330776a866e717f.jpg?thumb=1&w=720&h=360" mode=""></image>
				</view>
			</swiper-item><swiper-item>
				<view class="swiper-item">
					<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/1ab1ffaaeb5ca4c02674e9f35b1fd17c.jpg?thumb=1&w=720&h=360" mode=""></image>
				</view>
			</swiper-item><swiper-item>
				<view class="swiper-item">
					<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/a2b3ab270e5ae4c9e85d6607cdb97008.jpg?thumb=1&w=720&h=360" mode=""></image>
				</view>
			</swiper-item>
		</swiper>
		<view class="line"></view>
		<ul class="navList">
			<li><image src="../../../static/zhineng/bkxp.jpg"></image></li>
			<li><image src="../../../static/zhineng/xjd.webp.jpg"></image></li>
			<li><image src="../../../static/zhineng/shsb.webp.jpg"></image></li>
			<li><image src="../../../static/zhineng/ejyx.webp.jpg"></image></li>
			<li><image src="../../../static/zhineng/zndj.webp.jpg"></image></li>
			<li><image src="../../../static/zhineng/shjj.png"></image></li>
			<li><image src="../../../static/zhineng/qxcz.png"></image></li>
			<li><image src="../../../static/zhineng/jkqj.png"></image></li>
			<li><image src="../../../static/zhineng/etzq.png"></image></li>
			<li><image src="../../../static/zhineng/dyhc.png"></image></li>
		</ul>
		<view class="line"></view>
		<view class="rmbp">
			<image src="https://i8.mifile.cn/v1/a1/72411ddf-3df9-8d3a-7e5d-9429991710dc.webp" mode=""></image>
		</view>
		<view class="line"></view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="less" scoped>
	*{
		margin: 0;
		padding: 0;
	}
	.rmbp{
		image{
			height: 58.36 * 2rpx;
			width: 100%;
		}
	}
	.line{
		width: 100%;
		height: 16rpx;
		background-color: #fafafa;
	}
	.navList{
		display: flex;
		width: 100%;
		flex-wrap: wrap;
		li{
			flex: 20%;			
			list-style: none;
			image{
				width: 75.04 * 2rpx;
				height: 79.2rpx * 2;
			}
		}
	}
swiper{
	width: 100%;
	height: 187.5*2rpx;
	.swiper-item{
		image{
			width: 100%;
			height: 187.5 * 2rpx;
		}
	}
}
</style>
