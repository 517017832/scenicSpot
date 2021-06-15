<template>
	<view class="bg">
		<view class="content"></view>
		<tapBar />
	</view>
</template>

<script>
	import tapBar from "@/components/tab-bar"
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		components:{
			tapBar
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.bg{
		height: 100%;
	}
	.content {
		padding: 0 0 40px 0;
		height: 100%;
	}
</style>
