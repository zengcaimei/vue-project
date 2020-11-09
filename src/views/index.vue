<template>
	<div class="content">
		<p>vue3.0脚手架封装</p>
	</div>
</template>

<script>
	import {
		getListAPI
	} from '@/api/api'
	export default {
		data(){
			return{
				
			}
		},
		created() {
			this.getList()
		},
		methods:{
			getList(){
				getListAPI().then(res=>{
					console.log(res)
				})
			}
		}
	}
</script>

<style scoped lang="scss">
	.content{
		p{
			text-align: center;
		}
	}
</style>
