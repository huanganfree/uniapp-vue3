<template>
	<up-tabbar :value="active">
	  <up-tabbar-item @click="() => change(item)" :text="item.title" :icon="item.icon" :name="item.name" v-for="(item,index) in tabBarList" :key="item.name"></up-tabbar-item>
	</up-tabbar>
</template>

<script>
	export default {
		props: {
			active: {
				type: String,
				default: 'index'
			},
		},
		data() {
			return {
				tabBarList: [
					{
						name: 'index',
						path: '/pages/index/index',
						title: '首页',
						icon: 'home'
					},
					{
						name: 'my',
						path: '/pages/my/my',
						title: '我的',
						icon: 'account'
					}
				]
			}
		},
		created() {
		},
		methods: {
		  change({path, name}) {
			uni.switchTab({
				url:path
			})
		  }
		}
	}
</script>

<style lang="scss" scoped>

</style>
