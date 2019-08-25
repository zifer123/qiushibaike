<template>
	<view class="avatar">
		<image :src="src" :mode="mode" />
	</view>
</template>

<script>
	export default {
		name: 'Avatar',
		props: {
			src: {
				type: String,
				default: '',
			},
			mode: {
				type: String,
				default: 'widthFix',
			}
		},
		data() {
			return {
				
			};
		}
	}
</script>

<style scoped>
  .avatar {
		width: 90upx;
		height: 90upx;
		border-radius: 50%;
	}
	.avatar image {
		width: 100%;
		height: 100% !important;
		border-radius: 50%;
	}
</style>
