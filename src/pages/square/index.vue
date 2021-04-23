<template>
	<wuc-tab :tab-list="tabList" :tabCur.sync="TabCur" @change="tabChange"></wuc-tab>
</template>

<script>
	import WucTab from '/components/wuc-tab/wuc-tab.vue';

	export default {
		data() {
			return {
			TabCur: 0,
			tabList: [{
				name: '广场'
			}, {
				name: '推荐'
			}],
		}},
		components: { WucTab },
		methods: {
			tabChange(index) {
				this.TabCur = index;
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin: 200rpx auto 50rpx auto;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
