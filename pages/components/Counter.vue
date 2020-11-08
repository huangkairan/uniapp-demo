<template>
	<view class="content">
		<view class="text">
			<text>{{counter}}</text>
		</view>
		<view class="button">
			<button class="btn" type="default" @click="increment">+</button>
			<button class="btn" type="default" @click="decrement">-</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				counter: 0
			}
		},
		methods: {
			increment() {
				this.counter++;
			},
			decrement() {
				this.counter--;
			}
		}
	}
</script>

<style>
	.button{
		display: flex;
		.btn{
			flex:1
		}
	}
</style>
