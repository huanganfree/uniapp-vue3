<template>
  <view class="content">
      我的
	  <custom-tabbar :active="activeName" />
  </view>
</template>

<script>
export default {
  data() {
    return {
		activeName: 'my'
    }
  },
  onLoad() { },
  methods: {},
}
</script>

<style scoped lang="scss">

</style>
