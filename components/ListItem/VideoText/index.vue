<template>
	<view class="z-flex-fd-column wrapper" :style="{paddingLeft: paddingLeft + 'px', paddingRight: paddingRight + 'px'}">
		<view class="z-flex-ai-center header">
			<view class="z-flex-ai-center header-left">
				<Avatar src="/static/avatars/1.jpg" />
				<text class="username">丫丫</text>
			</view>

			<view class="z-flex-ai-center header-right">
				<view class="follow">+ 关注</view>
				<Icon type="guanbi" class="close" />
			</view>
		</view>

		<view class="title">
			如何用首长
		</view>

		<view class="image-wrapper">
			<image class="image" src="/static/dataPic/1.jpg" mode="widthFix"></image>
			<Icon type="bofang" class="play-button" :size="140" color="#FFFFFF" />
			<view class="play-info">20w次播放 02:24</view>
		</view>

		<view class="z-flex-jc-sb footer">
			<view class="z-flex-ai-center footer-left">
				<IconText type="dianzan1" :marginRight="14" />
				<IconText type="dianzan" />
			</view>
			
			<view class="z-flex-ai-center footer-right">
				<IconText type="huifu1" :marginRight="14" />
				<IconText type="huifu" />
			</view>
		</view>
	</view>
</template>

<script>
	import Icon from '../../Icon/index.vue';
	import Avatar from '../../Avatar.vue';
	import IconText from '../../IconText/index.vue';
	export default {
		name: 'videoTextItem',
		components: {
			Icon,
			Avatar,
			IconText,
		},
		props: {
			paddingLeft: {
				type: Number,
				default: 12,
			},
			paddingRight: {
				type: Number,
				default: 12,
			}
		},
	}
</script>

<style scoped>
	.wrapper {
		padding-top: 24upx;
		padding-bottom: 24upx;
		border-bottom: 1px solid #D5D5D5;
	}
	/* S = Header */
	.header {
		justify-content: space-between;
	}
	.header-left .username {
		margin-left: 16upx;
		font-size: 16px;
		letter-spacing: 2px;
		color: #A3A3A3;
	}

	.header-right .follow {
		background-color: #F4F4F4;
		padding: 2px 6px;
		border-radius: 1px;
		font-size: 12px;
		color: #333;
	}
	.header-right .close {
		margin-left: 20upx;
		font-size: 12px;
		color: #D6D6D6;
		padding: 6upx;
	}
	/* E = Header */
	
	/* S = 正文描述 */
	.title {
		margin-top: 20upx;
		margin-bottom: 20upx;
		color: #1B1B1B;
		font-weight: 400;
		letter-spacing: 1px;
	}
	/* E = 正文描述 */
	
	/* S = 图片 */
	.image-wrapper {
		position: relative;
		height: 470upx;
		margin-bottom: 40upx;
	}
	.image-wrapper image {
		width: 100%;
		height: 100% !important;
		border-radius: 10upx;
	}
	.image-wrapper .play-button {
		position: absolute;
		left: 50%;
		top: 50%;
		transform: translate(-50%, -50%);
	}
	.image-wrapper .play-info {
		position: absolute;
		bottom: 4upx;
		right: 4upx;
		font-size: 24upx;
		border-radius: 24upx;
		color: #FFFFFF;
		background-color: rgba(55, 55, 55, .72);
		padding: 4upx 12upx;
	}
	/* E = 图片 */
	
	/* S = 底部 */
	.footer {
		padding: 0 12upx;
	}
	.footer-left {
		
	}
	/* E = 底部 */
</style>
