<template>
	<view class="content">
        <uni-password ref="secrity" @input="onInput" @confirm="onConfirm">
        	请为账号****设置6位支付密码
        </uni-password>
	</view>
</template>

<script>
	import uniPassword from '@/components/uni-password/uni-password.vue'
	export default {
		components: {
			uniPassword
		},
		data() {
			return {
				
			}
		},
		onLoad() {

		},
		methods: {
			onInput(e) {
				//e.cancel = true;
			},
			onConfirm(e) {
				let password = e.value;
			}
		}
	}
</script>

<style>
	.content {
		text-align: center;
		height: 400upx;
	}
    .logo{
        height: 200upx;
        width: 200upx;
        margin-top: 200upx;
    }
	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
</style>
