<template>
	<view>
		<view class="header">
			<view class="logo">
				<image src="../../static/img/logo.png" mode=""></image>
			</view>
			<view class="search">
				<image src="../../static/img/search.png" ></image>
				<text>搜索商品名称</text>
			</view>
			<view class="user">
				<image src="../../static/icon/user.png" mode=""></image>
			</view>
		</view>
		<view class="nav">
			<ul>
				<li><text class="active">推荐</text></li>
				<li><text>手机</text></li>
				<li><text>智能</text></li>
				<li><text>电视</text></li>
				<li><text>家电</text></li>
				<li><text>笔记本</text></li>
			</ul>
		</view>
		<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000" 
		indicator-active-color="#fff" indicator-color="#ccc">
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/img/K40.jpg"></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/img/mifold.jpg" mode=""></image>
				</view>
			</swiper-item>
		</swiper>
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

<style lang="less">
	* {
		margin: 0;
		padding: 0;
	}
	swiper{
		width: 100%;
		height: 187.5*2rpx;
	}
	.swiper-item{
		image{
			width: 100%;
			height: 187.5*2rpx;
		}
	}
	.nav{
		width: 100%;
		background-color: #f2f2f2;
		ul{
			display: flex;
			width: 100%;
			height: 60rpx;
			li{
				display: flex;
				justify-content: center;
				align-items: center;
				flex-grow: 1;
				list-style: none;
				text{
					color: #747474;
					box-sizing: border-box;
					line-height: 60rpx;
					font-size: 28rpx;
					height: 60rpx;
				}
				.active{
					color: #ff6700;
					border-bottom: 1rpx solid #ff6700;
				}
			}
		}
	}
	.header {
		width: 100%;
		height: 43.76*2rpx;
		display: flex;
		align-items: center;
		background-color: #f2f2f2;

		.logo {
			display: flex;
			height: 100%;
			width: 52.09*2rpx;
			justify-content: center;
			align-items: center;

			image {
				width: 25*2rpx;
				height: 16.44*2rpx;
			}
		}
		.user {
			width: 52.09*2rpx;
			height: 31.26*2rpx;
			display: flex;
			justify-content: center;
			align-items: center;
			image {
				width: 20*2rpx;
				height: 20*2rpx;
			}
		}
		.search{
			border-radius: 4rpx;
			flex-grow: 1;
			height: 33.26*2rpx;
			background-color: #FFFFFF;
			display: flex;
			color: #b2b2b2;
			align-items: center;
			image{
				margin: 0 10rpx;
				width: 20*2rpx;
				height: 20*2rpx;
			}
		}

	}
</style>
