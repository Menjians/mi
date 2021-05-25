<template>
	<view class="outcontainer"> 
		<view class="line"></view>
		<view class="zbtj">
			<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/1bc92bd7fdb80c023c6887ae4f419e71.jpg?f=webp" mode=""></image>
		</view>
		<view class="line"></view>
		
		<view>
			<view class="big">
				<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b40029067abdfcc40bb6bde90b5d95d8.jpg?thumb=1&w=696&h=436" mode=""></image>
			</view>
			<view class="content">
					<view class="view1">
						<view class="name">RedmiBook Air 13</view>
						<view class="price">
							<text class="price-now">￥4799起</text>
							<text class="pre">￥5199</text>
						</view>
					</view>
					<view class="view2">
						<text>打开它，就像翻开一本杂志</text>
						<view class="btn">
							立即购买
						</view>
					</view>
			</view>
		</view>
		<view class="mtop">
			<view class="big">
				<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/84771bd0e6146ecbb6479735a4263ed5.jpg?thumb=1&w=696&h=436" mode=""></image>
			</view>
			<view class="content">
					<view class="view1">
						<view class="name">小米显示器 27英寸 165Hz版</view>
						<view class="price">
							<text class="price-now">￥2199</text>
						</view>
					</view>
					<view class="view2">
						<text>超广色域震撼影音，超清高刷畅爽电竞</text>
						<view class="btn">
							立即购买
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
	*{
		margin: 0;
		padding: 0;
	}
	.mtop{
		margin-top: 15rpx;
	}
	.outcontainer{
		background-color: #4878A6;
		padding: 0 12rpx;
		.content{
			height: 73.34 * 2rpx;
			width: 100%;
			background-color: #fff;
			box-sizing: border-box;
			padding: 20rpx 30rpx;
			.view1,.view2{
				display: flex;
				justify-content: space-between;
			}
			.view1{
				.name{
					color: #202020;
				}
				.price{
					.price-now{
						color: #EA625B;
						margin-right: 8rpx;
						font-size: 26rpx;
						font-weight: bold;
					}
					.pre{
						font-size: 24rpx;
						color: #757575;
						text-decoration: line-through;
					}
				}
			}
			.view2{
				height: 30.66*2rpx;
				text{
					font-size: 20rpx;
					color: #757575;
					line-height: 30.66 * 2rpx;
				}
				.btn{
					width: 103 * 2rpx;
					height: 60rpx;background-color: #ea625b;
					border-radius: 6rpx;
					text-align: center;
					line-height: 60rpx;
					color: #fff;
					font-size: 26rpx;
				}
			}
		}
		
		.big{
			image{
				width: 100%;
				height: 227 * 2rpx;
				vertical-align: bottom;
			}
		}
		.zbtj{
			image{
				width: 100%;
				height: 41.66 * 2rpx;
				vertical-align: bottom;
			}
		}
		.line{
			width: 100%;
			height: 28rpx;
			background-color: #4878A6;
		}
	}
	

</style>
