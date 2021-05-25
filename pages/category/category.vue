<template>
	<view class="outer">
		<view class="header">
			<view class="back" @tap="back()">
				<image src="../../static/icon/back.png" mode=""></image>
			</view>
			<view class="title">分类</view>
			<view class="search">
				<image src="../../static/img/search.png" mode=""></image>
			</view>
		</view>
		<view class="container">
			<scroll-view scroll-y="true" class="scroll-left">
				<view class="item" v-for="(item,index) in itemList" :key="index">{{item}}</view>
			</scroll-view>
			<scroll-view scroll-y="true" class="scroll-right">
				<view class="title">
					<image src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/43c675e2416837f1f5fe60daa7698475.jpg?f=webp&w=750&h=300&bg=F99E69" mode=""></image>
				</view>
				<view v-for="(item,index) in cate_list" :key="index">
					<view class="cate_title">
						{{item.title}}
					</view>
					<ul class="cate_list">
						<li v-for="item in item.listItems">
							<image :src="item.img" ></image>
							<view class="name">{{item.name}}</view>
						</li>
					</ul>
				</view>
				
			</scroll-view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				itemList:['小米手机','Redmi手机','游戏手机','智能穿戴','电视','电脑办公','大家电','小家电','智能家居','户外出行','日用百货','儿童用品','小米服务','零售店'],
				cate_list:[
					{
						title:"小米数字系列",
						listItems:[
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/c9d21c3752a74ae29b7f949ee977badd.png?thumb=1&w=120&h=120",name:"小米11 Ultra"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/d3a36269683536a9d46a044392ed37ab.png?thumb=1&w=120&h=120",name:"小米11 Pro"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b0e55e428c57a718fd87d23cce939637.png?thumb=1&w=120&h=120",name:"小米11青春版"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/2768f0ffc7d8dd66e5c58c9062898338.png?thumb=1&w=120&h=120",name:"小米10S"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/9732a817c834a5002e3ee5b7947e00ec.png?thumb=1&w=120&h=120",name:"小米11"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/2a47c566e14b2da1a6cc0780060a59d0.png?thumb=1&w=120&h=120",name:"小米10 至尊版"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/58a4446432aba7894e957f2c18853562.png?thumb=1&w=120&h=120",name:"小米10 青春"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/acf2e521e29e5afabf6d493203b31f27.png?thumb=1&w=120&h=120",name:"小米10"}
						]
					},
					{
						title:"小米MIX系列",
						listItems:[
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/acf2e521e29e5afabf6d493203b31f27.png?thumb=1&w=120&h=120",name:"MIX FOLD"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/266ad6dd5146deaf3ae3602a89e7a217.png?thumb=1&w=120&h=120",name:"MIX Alpha"}
						]
					},
					{
						title:"小米手机配件",
						listItems:[
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/901c89ad5e92c6408980decd7a79b739.png?thumb=1&w=120&h=120",name:"无线充"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/ce7aaeec82e51a44790959295183f669.png?thumb=1&w=120&h=120",name:"充电器"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/445044cfe12a08c38835d5adba07b5a1.png?thumb=1&w=120&h=120",name:"数据线"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/8070925c6ba4d476392499454b973ff8.png?thumb=1&w=120&h=120",name:"小米充电宝"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/299b5373e77b8ad1f315db3a997c8728.png?thumb=1&w=120&h=120",name:"小米手机保护壳"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/7c53333674a3c8ddcad980525f2842c9.png?thumb=1&w=120&h=120",name:"小米手机贴膜"}
						]
					},
					{
						title:"Redmi红米 Note系列",
						listItems:[
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/4a05330038898964f80945746ebeec5b.png?thumb=1&w=120&h=120",name:"Note 9 Pro"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/f1f3f7877ff788e9f891ada601f2996c.png?thumb=1&w=120&h=120",name:"Note 9"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/9f4c188f619f4ee7bca4a09de987691e.png?thumb=1&w=120&h=120",name:"Note 9 4G"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/99022ce28f145ff5a521c848596295ec.gif",name:"Note 8 Pro"},
							{img:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/271b3bd052e735143ee7298f2d6d43fa.gif",name:"Redmi Note 8"},
						]
					}
				]
			}
		},
		methods: {
			back(){
				uni.navigateBack()
			}
		}
	}
</script>

<style lang="less" scoped>
*{
	margin: 0;
	padding: 0;
}
page{
	height: 100%;
	padding-top: 100rpx;
}
.outer{
	height: 100%;
	.container{
			display: flex;
			width: 100%;
			height: calc(100vh - 200rpx);
			padding-right:20rpx ;
			.cate_title{
				width: 262.52 * 2rpx;
				height: 66.66 * 2rpx;
				display: flex;
				justify-content: center;
				align-items: center;
				box-sizing: border-box;
				font-size: 30rpx;
			}
			.cate_title::before,.cate_title::after{
				content: "";
				width: 20.83*2rpx;
				height: 4rpx;
				background-color: #EFEFEF;
			}
			.cate_title::before{
				margin-right: 20rpx;
			}
			.cate_title::after{
				margin-left: 20rpx;
			}
			.scroll-left{
				width: 25%;
				box-sizing: border-box;
				border-right: 1rpx solid #eee;
				.item{
					width: 100%;
					height: 90rpx;
					line-height: 90rpx;
					font-size: 28rpx;
					text-align: center;
					color: #3c3c3c;
				}
			}
			.scroll-right{                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      
				width: 75%;
				display:border-box;
				padding: 0 30rpx;
				.title{
					image{
						width:260 * 2rpx ;
						height: 104*2rpx;
					}
				}
				.cate_list{
					box-sizing: border-box;
					display: flex;
					flex-wrap: wrap;
					li{
						flex: 33.33%;
						flex-grow: unset;
						display: flex;
						flex-direction: column;
						justify-content: center;
						align-items: center;
						margin-bottom: 40rpx;
						image{
							width: 52.08 * 2rpx;
							height: 52.08 * 2rpx;
						}
						.name{
							width: 87.5 * 2rpx;                        
							height: 13 * 2rpx;
							font-size: 20rpx;
							text-align: center;
							margin-top: 20rpx;
						}
					}
				}
			}
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
