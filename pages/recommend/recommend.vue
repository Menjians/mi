<template>
	<view>
		<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000" indicator-active-color="#fff"
			indicator-color="#ccc">
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
			<li>
				<image src="../../static/imgnav/xmms.png" mode=""></image>
			</li>
			<li>
				<image src="../../static/imgnav/xmzc.webp.jpg">
			</li>
			<li>
				<image src="../../static/imgnav/Note9.webp.jpg">
			</li>
			<li>
				<image src="../../static/imgnav/yjhx.webp.jpg">
			</li>
			<li>
				<image src="../../static/imgnav/xmsx.webp.jpg">
			</li>
			<li>
				<image src="../../static/imgnav/zn.webp.jpg">
			</li>
			<li>
				<image src="../../static/imgnav/bjbrm.png">
			</li>
			<li>
				<image src="../../static/imgnav/dsrm.png">
			</li>
			<li>
				<image src="../../static/imgnav/xyjrm.webp.jpg">
			</li>
			<li>
				<image src="../../static/imgnav/mfk.png">
			</li>
		</ul>
		<view class="divider"></view>
		<view class="container">
			<view class="viewleft">
				<image
					src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/29b39579739d82269d18f0e7c8f6c9da.jpg?f=webp&w=537&h=762&bg=57524C">
				</image>
			</view>
			<view class="viewright">
				<image
					src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/5b9af94e5c05bb2b4849cbb113eddb9d.jpg?f=webp&w=537&h=378&bg=EBF8FF">
				</image>
				<image
					src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/42e02f30c05282812529e499211f4c85.png?f=webp&w=537&h=378&bg=E9F7FF">
				</image>
			</view>
		</view>
		<view class="hot">
			<image
				src="http://cdn.cnbj1.fds.api.mi-img.com/mi-mall/5b2fff7f7b8de6d371601caf3a827eed.jpg?f=webp&w=1080&h=660&bg=F5F5F5"
				mode=""></image>
		</view>
		<view class="shouji">
			<view class="sj-left">
				<view class="sj-left-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b849e46756af7c95002aa3906ed77c13.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-left-bottom">
					<text class="sj-name">小米11 Pro</text>
					<text class="sj-num">1.12''GN2｜骁龙888</text>
					<text class="sj-price">￥4999起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
			<view class="sj-right">
				<view class="sj-right-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/94b22bbff9fa84440a0aed48f9f63154.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-right-bottom">
					<text class="sj-name">MIX FOLD 小米折叠屏手机</text>
					<text class="sj-num">折叠大屏｜自研芯片</text>
					<text class="sj-price">￥9999起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
		</view>
		<view class="shouji">
			<view class="sj-left">
				<view class="sj-left-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/6dca45286d9d76d1f864a8ecf77f5600.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-left-bottom">
					<text class="sj-name">Note 9 5G</text>
					<text class="sj-num">天玑 800U处理器，5000mAh电池，</text>
					<text class="sj-price">￥1299起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
			<view class="sj-right">
				<view class="sj-right-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/455c8ad8d204e4ffd67865a98ae40c7b.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-right-bottom">
					<text class="sj-name">小米10S</text>
					<text class="sj-num">骁龙870 | 对称式双扬立体声</text>
					<text class="sj-price">￥3299起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
		</view>
		<view class="shouji">
			<view class="sj-left">
				<view class="sj-left-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b32136fc8b4e81e8bca912d23c384c9d.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-left-bottom">
					<text class="sj-name">Note 9 Pro 5G</text>
					<text class="sj-num">一亿像素夜景相机，120Hz六档变速高刷屏</text>
					<text class="sj-price">￥1499起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
			<view class="sj-right">
				<view class="sj-right-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/931c518351d93186d11ab7548a2754b5.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-right-bottom">
					<text class="sj-name">小米11</text>
					<text class="sj-num">骁龙888 | 2K四曲面屏</text>
					<text class="sj-price">￥3999起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
		</view><view class="shouji">
			<view class="sj-left">
				<view class="sj-left-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/7fb74299ef995a4ae4f4a687c9873f78.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-left-bottom">
					<text class="sj-name">黑鲨4</text>
					<text class="sj-num">黑鲨4 磁动力升降肩键</text>
					<text class="sj-price">￥2499起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
			<view class="sj-right">
				<view class="sj-right-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/66976d8caaea76a1a14db103e2793897.jpg?thumb=1&w=344&h=280"
						mode=""></image>
				</view>
				<view class="sj-right-bottom">
					<text class="sj-name">Redmi  K40 Pro 系列</text>
					<text class="sj-num">骁龙888 / E4 旗舰直屏</text>
					<text class="sj-price">￥2799起</text>
					<button class="buybtn">立即购买</button>
				</view>
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
	* {
		margin: 0;
		padding: 0;
	}

	.shouji {
		width: 100%;
		display: flex;
		justify-content: space-between;
		height: 253.2 * 2rpx;

		.sj-left {
			margin-left: 10rpx;
		}

		.sj-right {
			margin-right: 10rpx;
		}

		.sj-left,
		.sj-right {
			width: 179.23 * 2rpx;
		}

		.sj-left-top,
		.sj-right-top {
			image {
				width: 179.25 * 2rpx;
				height: 145.9 * 2rpx;
			}

		}

		.sj-left-bottom,
		.sj-right-bottom {
			width: 179.25 * 2rpx;
			height: 107.3 * 2rpx;
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;

			.sj-name {
				font-size: 28rpx;
				width: 300rpx;
				height: 32rpx;
				text-align: center;
				white-space: nowrap;
				overflow: hidden;
				text-overflow: ellipsis;
			}

			.sj-num {
				width: 300rpx;
				height: 30rpx;
				text-align: center;
				white-space: nowrap;
				text-overflow: ellipsis;
				overflow: hidden;
				font-size: 24rpx;
				margin: 3rpx 0;
			}

			.sj-price {
				font-size: 28rpx;
				color: #EA625B;
			}

			.buybtn {
				width: 104.21 *2rpx;
				height: 30.28 * 2rpx;
				background-color: #EA625B;
				line-height: 30.28 * 2rpx;
				color: #fff;
				font-size: 26rpx;
			}
		}
	}

	.hot {
		image {
			width: 100%;
			height: 229.29*2rpx;
		}
	}

	.container {
		width: 100%;
		height: 264.71*2rpx;
		display: flex;
		justify-content: space-between;

		.viewleft,
		.viewright {
			width: 186.55*2rpx;
			height: 264.71*2rpx;
		}

		.viewleft {
			image {
				width: 186.55*2rpx;
				height: 264.71*2rpx;
			}
		}

		.viewright {
			display: flex;
			flex-direction: column;
			justify-content: space-between;

			image {
				width: 186.55*2rpx;
				height: 131.31*2rpx;
			}
		}
	}

	.divider {
		width: 100%;
		height: 8.34 * 2rpx;
		background: #f5f5f5;
	}

	.navList {
		display: flex;
		flex-wrap: wrap;

		li {
			list-style: none;
			flex: 20%;

			image {
				width: 75.04*2rpx;
				height: 79.02*2rpx;
			}
		}
	}

	swiper {
		width: 100%;
		height: 187.5*2rpx;
	}

	.swiper-item {
		image {
			width: 100%;
			height: 187.5*2rpx;
		}
	}
</style>
