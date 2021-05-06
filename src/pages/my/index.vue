<template>
	<view class="content">	
		<view>
			<u-navbar :is-back="false" title="我的瞬间" :background="background" title-color="#fff"></u-navbar>
		</view>
		<view class="avatar-div" :style="{background: 'url(' + imageURL + ') no-repeat center'}">
			<view class='avatar'>
				<u-avatar :src="src" bg-color="#eee" size="large"></u-avatar>
				<view style="color: #ffffff;margin: 1rem 0 0 0">墨星人</view>
				<view class="avatar-tab">
					<view class="avatar-tab-item">
						<u-tag text="吃货" shape="circle" bg-color="#ccc" border-color="#ccc" color="#fff" size="mini" />
					</view>
					<view class="avatar-tab-item">
						<u-tag text="吃货" shape="circle" size="mini" />
					</view>
					<view class="avatar-tab-item">
						<u-tag text="吃货" shape="circle" size="mini" />
					</view>
					<view class="avatar-tab-item">
						<u-tag text="吃货" shape="circle" size="mini" />
					</view>
					<view class="avatar-tab-item">
						<u-tag text="吃货" shape="circle" size="mini" />
					</view>
					<view class="avatar-tab-item">
						<u-tag text="吃货" shape="circle" size="mini" />
					</view>
					<view class="avatar-tab-item">
						<u-tag text="点击添加+" shape="circle" size="mini" />
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				background: {
					background: 'url(https://gimg2.baidu.com/image_search/src=http%3A%2F%2Finews.gtimg.com%2Fnewsapp_match%2F0%2F12020722655%2F0.jpg&refer=http%3A%2F%2Finews.gtimg.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1622812294&t=13bc6f545da69fad12cc0a76a429f1bf) no-repeat bottom',
				},
				src: null,
				text: '墨',
				imageURL: 'https://gimg2.baidu.com/image_search/src=http%3A%2F%2Finews.gtimg.com%2Fnewsapp_match%2F0%2F12020722655%2F0.jpg&refer=http%3A%2F%2Finews.gtimg.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1622812294&t=13bc6f545da69fad12cc0a76a429f1bf'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	/* 注意要写在第一行，同时给style标签加入lang="scss"属性 */
	@import "uview-ui/index.scss";
	.avatar-div {
		width: 100%;
		height: 13rem;
	}
	.avatar {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		padding: 2rem 0rem;
	}
	.avatar-tab {
		width: 70%;
		margin: 1rem;
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}
	.avatar-tab-item {
		padding: 0.1rem;
	}
</style>
