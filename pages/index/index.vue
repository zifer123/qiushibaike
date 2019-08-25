<template>
	<view class="index-wrapper">
		首页
		<VideoText />
		<ImageText />
		<ImageText />
		<ImageText />
		<ImageText />
	</view>
</template>

<script>
	import ImageText from '../../components/ListItem/ImageText/index.vue';
	import VideoText from '../../components/ListItem/VideoText/index.vue';
	export default {
		components: {
			ImageText,
			VideoText,
		},
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style scoped>
	.index-wrapper {
		
	}
</style>
