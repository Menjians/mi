<template>
	<view>
		<view class="xiaomi11">
			<image class="xiaomi11" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/c6cb8fc7a8a6136108adb4c8a79f8218.jpg?f=webp"></image>
		</view>
		<view class="line"></view>
		<view class="hot">
			<image class="hot" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/d41803630a405f2e7ac241f9bea260f4.jpg?f=webp" mode=""></image>
		</view>
		<view class="line"></view>
		<view class="note9">
			<image class="note9" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/8825bae3253a196aa1e9f6a8e5247b45.jpg?f=webp" mode=""></image>
		</view>
		<view class="line"></view>
		<view class="miqc">
			<image class="miqc" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/88589308a12c8495fdc671320840a379.jpg?f=webp" mode=""></image>
		</view>
		<view class="line"></view>
		<view class="kjtt">
			<image class="kjtt" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/20c641a195013740256f0de2a2d04f90.jpg?f=webp" mode=""></image>
		</view>
		<view class="line"></view>
		<view class="szml">
			<image class="szml" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/188d21cb0a7600f24a7eab2e2d720739.jpg?f=webp" mode=""></image>
		</view>
		<view class="line"></view>
		<view class="shouji">
			<view class="sj-left">
				<view class="sj-left-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/24d83fd2f53cc48f55b85e8b34f2a652.jpg?thumb=1&w=338&h=338"
						mode=""></image>
				</view>
				<view class="sj-left-bottom">
					<text class="sj-name">Redmi 9A</text>
					<text class="sj-num">5000mAh长循环大电量，6.53"超大护眼屏幕，大音量扬声器</text>
					<text class="sj-price">￥499起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
			<view class="sj-right">
				<view class="sj-right-top">
					<image
						src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/73f13cecbb9e9c9ff78a9ee6dae5ad8b.jpg?thumb=1&w=338&h=338"
						mode=""></image>
				</view>
				<view class="sj-right-bottom">
					<text class="sj-name">Redmi 10X 4G</text>
					<text class="sj-num">5020mAh超长续航，128GB大内存，4800万超清四摄</text>
					<text class="sj-price">￥999起</text>
					<button class="buybtn">立即购买</button>
				</view>
			</view>
		</view>
		<view class="line"></view>
		<view class="more">
			<image class="more" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/81ab8e922b2a5948ad33b6984beaf216.jpg?f=webp" mode=""></image>
		</view>
		<view class="line"></view>
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

<style lang="less" scoped>
*{
	margin: 0;
	padding: 0;
}
.more{
	width: 100%;
	height: 57.28*2rpx;
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
.szml{
	width: 100%;
	height: 57.31*2rpx;
}
.kjtt{
	width: 100%;
	height: 52.81*2rpx;
}
.miqc{
	width: 100%;
	height: 273.58rpx * 2;
}
.note9{
	width: 100%;
	height: 275* 2rpx;
}
.xiaomi11{
	vertical-align: bottom;
	image{
		width: 100%;
		height: 408.55*2rpx;
	}
	}
.line{
	width: 100%;
	height: 16rpx;
	background-color: #DCE6F2;
}
.hot{
	width: 100%;
	height: 44.81*2rpx;
}
</style>
