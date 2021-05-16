<template>
	<view class="outer">
		<view class="header">
			<view class="back">
				<image src="../../static/icon/back.png" mode=""></image>
			</view>
			<view class="title">分类</view>
			<view class="search">
				<image src="../../static/img/search.png" mode=""></image>
			</view>
		</view>
		<view class="container">
			<view class="left">
				<scroll-view scroll-y="true" class="scroll-left">
					<view class="item" v-for="(item,index) in itemList" :key="index">{{item}}</view>
				</scroll-view>
			</view>
			<view class="right">
				<scroll-view scroll-y="true" class="scroll-right">
					<view></view>
				</scroll-view>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				itemList:['小米手机','Redmi手机','游戏手机','智能穿戴','电视','电脑办公','大家电','小家电','智能家居','户外出行','日用百货','儿童用品','小米服务','零售店']
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
.container{
	display: flex;
	margin-top: 100rpx;
	height: 100%;
	.left{
		width: 25%;
		height: 100%;
		box-sizing: border-box;
		border-right: 1rpx solid #eee;
		padding-top: 30rpx;
		.scroll-left{
			height: calc(100vh - 100rpx);
			.item{
				width: 100%;
				height: 90rpx;
				line-height: 90rpx;
				font-size: 28rpx;
				text-align: center;
				color: #3c3c3c;
			}
		}
	}
	.right{
		height: 100%;
		width: 75%;
	}
}
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
