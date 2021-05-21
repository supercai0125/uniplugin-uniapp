<template>
	<view class="container">
		<button type="default" @click="watchUpdate">手表更新</button>
	</view>
</template>

<script>
	var PhoneBle = uni.requireNativePlugin("Phone-Ble");
	export default {
		methods: {
			watchUpdate() {
				PhoneBle.gotoNativePage()
			},
		}
	}
</script>

<style>
	.container {
		padding: 20px;
		font-size: 14px;
		line-height: 24px;
	}
</style>
