<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view><Title></Title></view>
	</view>
</template>

<script>
import add from '../../utils/add.js';
import Title from '../../components/Title/Title.vue';
export default {
	components: {
		Title
	},
	data() {
		return {
			title: 'Hello'
		};
	},
	onLoad() {
		console.log(add(4, 5));
	},
	methods: {}
};
</script>

<style lang="scss">
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
