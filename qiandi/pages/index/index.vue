<template>
	<view class="content">
		<!-- 轮播广告 -->
		<coursel></coursel>
		<!-- 楼层导航 -->
		<view class="loucen-list">
			<view class="loucen-item" v-for="(item,i) in loucenlist.loucen" :key="i">
				<view class="tupian">					
					<image :src="item.src" mode=""></image>
					<view class="wenzi uni-h5">{{item.title}}</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import coursel from "../../components/coursel.vue"
	import loucen from "../../messagelist.json"
	export default {
		components:{
			coursel
		},
		data() {
			return {
				loucenlist:loucen
			}
		},
		onLoad() {
			
		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.content {
		.loucen-list{
			margin:20rpx 0;
			display: flex;
			justify-content: space-around;
			.loucen-item{
				text-align: center;
				.tupian{
					image{
						width:90rpx;
						height:90rpx;
					}
				}
			}
		}
	}
</style>
