<template>
	<view class="z-flex-ai-center" :style="{marginRight: marginRight + 'px'}" @click="handleClick">
		<Icon :type="type" :color="color" />
		<text class="num" :style="{color: color}">{{ num }}</text>
	</view>
</template>

<script>
	import Icon from '../Icon/index.vue';
	export default {
		name: 'IconText',
		components: {
			Icon,
		},
		props: {
			type: {
				type: String,
				default: '',
			},
			color: {
				type: String,
				default: '#D5D5D5',
			},
			num: {
				type: Number,
				default: 0,
			},
			marginRight: {
				type: [Number, String],
				default: 0,
			},
		},
		methods: {
			handleClick() {
				this.$emit('click');
			}
		}
	}
</script>

<style scoped>
	.num {
		margin-left: 24upx;
	}
</style>
