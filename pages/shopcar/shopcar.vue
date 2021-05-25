<template>
	<view>
		<view class="header">
			<view class="back">
				<image src="../../static/icon/back.png" mode=""></image>
			</view>
			<view class="title">购物车</view>
			<view class="search">
				<image src="../../static/img/search.png" mode=""></image>
			</view>
		</view>
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
.header{
	width: 100%;
	height: 100rpx;
	position: fixed;
	z-index: 1;
	top: 0;
	left: 0;
	background-color: #f2f2f2;
	display: flex;
	align-items: center;
	.title{
		flex-grow: 1;
		text-align: center;
		color: #666;
	}
	.back{
		display: flex;
		justify-content: center;
		align-items: center;
		width: 52.09 * 2rpx;
		height: 26.05 * 2rpx;
		image{
			width: 52rpx;
			height: 52rpx;
		}
	}
	.search{
		width: 52 * 2rpx;
		height: 31.26*2rpx;
		display: flex;
		justify-content: center;
		align-items: center;
		image{
			width: 31.26 * 2rpx;
			height: 31.26 * 2rpx;
		}
	}
}
</style>
