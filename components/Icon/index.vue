<template>
	<view class="iconfont" :class="'icon-' + type" :style="{color: color, 'font-size': size + 'upx'}" @tap="onClick"></view>
</template>

<script>
	export default {
		name: 'iconfont',
		props: {
			type: {
				type: String,
				default: '',
			},
			color: {
				type: String,
				default: '#D6D6D6',
			},
			size: {
				type: [String, Number],
				default: 32,
			}
		},
		methods: {
			onClick() {
				this.$emit('click');
			},
		},
	}
</script>

<style>
</style>
