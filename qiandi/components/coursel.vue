<template>
	<view class="coursel">
		<swiper class="swiper" indicator-dots="true" autoplay="true" interval="3000" duration="500" indicator-active-color="#fff" circular="true">
			<swiper-item v-for="(item,i) in clist.coursel" :key="i">
					<view class="swiper-item">
						<image :src="item.img" mode=""></image>
					</view>
			</swiper-item>
		</swiper>
	</view>
</template>

<script>
	import clist from "../messagelist.json"
	export default{
		data(){
			return{
				clist:clist
			}
		},
		methods:{
			
		}
	}
</script>

<style lang="scss">
	.coursel{
		.swiper{
			.swiper-item{
				image{width:100%;height:300rpx;}
			}
		}
	}
</style>
