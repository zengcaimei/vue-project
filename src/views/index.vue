<template>
	<div class="content">
		<p>维康大药房（广州）有限公司线上实时运营数据</p>
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
			font-size: 0.325rem;
			font-weight: bold;
		}
	}
</style>
