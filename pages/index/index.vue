<template>
	<view class="content">
		<view class="title">uniCloud 云函数示例</view>
		<view class="btn-list">
			<button type="primary" @click="goto('mpweixinLogin')">微信小程序登录</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {}
		},
		methods: {
			goto(name) {
				uni.navigateTo({
					url: `/pages/${name}/${name}`
				})
			}
		}
	}
</script>

<style>
	.title {
		font-weight: bold;
		text-align: center;
		padding: 20px 0px;
		font-size: 20px;
	}

	.tips {
		color: #999999;
		font-size: 14px;
		padding: 20px 30px;
	}

	.btn-list {
		padding: 0px 30px;
	}

	.btn-list button {
		margin-bottom: 20px;
	}
</style>
