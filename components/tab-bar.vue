<template>
	<!-- <van-tabbar v-model="active" @change="handleMenu">
		<van-tabbar-item 
			v-for="(item, index) in tabBar.list" 
			:key="index" icon="home-o" badge="item.badge" :dot="item.dot"
		>{{item.text}}
		</van-tabbar-item>
	</van-tabbar> -->
	<van-tabbar v-model="active">
	  <van-tabbar-item icon="home-o">标签</van-tabbar-item>
	  <van-tabbar-item icon="search" dot>标签</van-tabbar-item>
	  <van-tabbar-item icon="friends-o" badge="5">标签</van-tabbar-item>
	  <van-tabbar-item icon="setting-o" badge="20">标签</van-tabbar-item>
	</van-tabbar>
</template>

<script>
	export default {
		name:"tab-bar",
		data() {
			return {
				active: 0, //当前激活的菜单index
				tabBar: {
					list: [{
						pagePath: '/pages/homePage/homePage',
						text: '首页',
						dot: "", //红色提示
						badge: "" //红色数字
					}, {
						pagePath: '/pages/mine/mine',
						text: '我的',
						dot: "",
						badge: "3"
					}]
				}
			};
		},
		methods:{
			handleMenu(index) {
				this.active = index
			}
		}
	}
</script>

<style lang="scss">
.content{
	.menu{
		
	}
}
</style>
