<template>
  <view class="content">
    <up-button text="月落" class="reset-button"></up-button>
    <up-button type="primary" :plain="true" text="镂空12"></up-button>
    <custom-tabbar active="index"/>
  </view>
</template>

<script>
export default {
  data() {
    return {
    }
  },
	onLoad(){
		console.log('index--onload')
	},
  methods: {
  },
}
</script>

<style scoped lang="scss">

</style>
