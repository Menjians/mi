<template>
	<view class="container">
		<view class="start">
			<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/5a56b920bc83820736d2260c58858bf4.jpg?f=webp" mode=""></image>
		</view>
		<view class="hotbp">
			<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/206eeb5a11b27d97cec3f2b2c053a083.jpg?f=webp" mode=""></image>
		</view>
		
		<view class="Tvlist">
			<view>
				<view class="smallimg">
					<view class="pos">
						<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/20d970b239e6b7152d07b6282e160192.jpg?thumb=1&w=221&h=221" mode=""></image>
						<image class="mx" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/57817f3ee2b04f655c5d98c255ed9a9a.png?w=167&h=167" mode=""></image>
					</view>
				</view>
				<view class="info">
					<text class="name">全面屏E32C</text>
					<text class="text">全面屏设计，人工智能系统</text>
					<view>
						<text class="price">¥949</text> <text class="old-price">¥1099</text>
					</view>
				</view>
			</view>
			<view>
				<view class="smallimg">
					<view class="pos">
						<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/c1bb566a499a4691cf878bb3ac23c056.jpg?thumb=1&w=221&h=221" mode=""></image>
						<image class="mx" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/57817f3ee2b04f655c5d98c255ed9a9a.png?w=167&h=167" mode=""></image>
					</view>
				</view>
				<view class="info">
					<text class="name">小米电视4A 70英寸</text>
					<text class="text">大屏更享受</text>
					<view>
						<text class="price">¥3688</text> <text class="old-price">¥3999</text>
					</view>
				</view>
			</view>
			<view>
				<view class="smallimg">
					<view class="pos">
						<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/abf7219dc5dd88a5a425e05d66459c1e.jpg?thumb=1&w=221&h=221" mode=""></image>
						<image class="mx" src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/57817f3ee2b04f655c5d98c255ed9a9a.png?w=167&h=167" mode=""></image>
					</view>
				</view>
				<view class="info">
					<text class="name">小米电视4A 60英寸</text>
					<text class="text">人工智能语音系统,超高清画质</text>
					<view>
						<text class="price">¥2788</text> <text class="old-price">¥2799</text>
					</view>
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
	.container{
		background-color: #E14139;
	}
image{
	vertical-align: bottom;
}
.Tvlist{
	display: flex;
	width: 100%;
	flex-wrap: wrap;
	margin: 0 16rpx;
	justify-content: space-between;
	.smallimg{
		width: 115.09 * 2rpx;
		height: 115.09 * 2rpx;
		.pos{
			image{
				width: 115.09 * 2rpx;
				height: 115.09 * 2rpx;
			}
			.mx{
				position: absolute;
				width: 52 * 2rpx;
				height: 52*2rpx;
				right: 2rpx;
				bottom: 5rpx;
			}
		}
	}
	.info{
		display: flex;
		background-color: #fff;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 115 * 2rpx;
		height: 75.42 * 2rpx;
		.price{
			color: #f54b4b;
			font-size: 17*2rpx;
			font-weight: bold;
		}
		.old-price{
			color: #464646;
			text-decoration: line-through;
			margin-left: 10rpx;
			font-size: 22rpx;
			font-weight: bold;
		}
		.name,.text{
			width: 104.63 * 2rpx;
			text-align: center;
			white-space: nowrap;
			overflow: hidden;
			text-overflow: ellipsis;
			color: #3c3c3c;
		}
		.text{
			font-size: 12.61*2rpx;
		}
		.name{
			font-weight: bold;
			font-size: 28rpx;
		}
	}
	
}
.start{
	image{
		width: 100%;
		height: 64.58 * 2rpx;
	}
}
.hotbp{
	image{
		width: 100%;
		height: 70.83 * 2rpx;	
	}
}
</style>
