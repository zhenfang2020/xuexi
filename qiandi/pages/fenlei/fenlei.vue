<template>
	<view class="fenlei">
		这里是分类
		<view>测试顶部固定高度，下拉出现滚动条</view>
		<view class="ceshi">
			<view class="guding" style="background-color: #007AFF;height:100px">我是固定不变的</view>
			<view class="container">
				<view class="bianhua">
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
					<view>啦啦啦房东送送你</view>
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

<style lang="scss">
	.fenlei{
		.ceshi{
			.guding{
				position:fixed;
				width:100%;height:auto;
				background:#ffc;
				overflow-y:auto;
				min-height: 60px;
				line-height: 60px;
			}
			.container{
				padding-top:60px;
				.bianhua{
					view{height: 150rpx;line-height: 150rpx;}
				}
			}
		}
	}
</style>
