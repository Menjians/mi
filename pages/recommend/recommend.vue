<template>
	<view>
		<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000"
		indicator-active-color="#fff" indicator-color="#ccc">
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/img/xiaomiUltra.jpg"></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/img/mifold.jpg" mode=""></image>
				</view>
			</swiper-item>
		</swiper>
		<ul class="navList">
			<li><image src="../../static/imgnav/xmms.png" mode=""></image></li>
			<li><image src="../../static/imgnav/xmzc.webp.jpg"></li>
			<li><image src="../../static/imgnav/Note9.webp.jpg"></li>
			<li><image src="../../static/imgnav/yjhx.webp.jpg"></li>
			<li><image src="../../static/imgnav/xmsx.webp.jpg"></li>
			<li><image src="../../static/imgnav/zn.webp.jpg"></li>
			<li><image src="../../static/imgnav/bjbrm.png"></li>
			<li><image src="../../static/imgnav/dsrm.png"></li>
			<li><image src="../../static/imgnav/xyjrm.webp.jpg"></li>
			<li><image src="../../static/imgnav/mfk.png"></li>
		</ul>
		<view class="divider"></view>
		<view class="container">
			<view class="viewleft">
				<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/29b39579739d82269d18f0e7c8f6c9da.jpg?f=webp&w=537&h=762&bg=57524C"></image>
			</view>
			<view class="viewright">
				<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/5b9af94e5c05bb2b4849cbb113eddb9d.jpg?f=webp&w=537&h=378&bg=EBF8FF"></image>
				<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/42e02f30c05282812529e499211f4c85.png?f=webp&w=537&h=378&bg=E9F7FF"></image>
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
	*{
		margin: 0;
		padding: 0;
	}
	.container{
		width: 100%;
		height: 264.71*2rpx;
		display: flex;
		justify-content: space-between;
		.viewleft,.viewright{
			width: 186.55*2rpx;
			height: 264.71*2rpx;
		}
		.viewleft{
			image{
				width: 186.55*2rpx;
				height: 264.71*2rpx;
			}
		}
		.viewright{
			display: flex;
			flex-direction: column;
			justify-content: space-between;
			image{
				width: 186.55*2rpx;
				height: 131.31*2rpx;
			}
		}
	}
	.divider{
		width: 100%;
		height: 8.34 * 2rpx;
		background: #f5f5f5;
	}
	.navList{
		display: flex;
		flex-wrap: wrap;
		li{
			list-style: none;
			flex: 20%;
			image{
				width: 75.04*2rpx;
				height: 79.02*2rpx;
			}
		}
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
</style>
