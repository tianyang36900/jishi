<template>
	<div>
		<div>
			<div id="box">
				<button>添加</button>
				<table>
					<tr>
						<td>学号</td>
						<td>姓名</td>
						<td>年龄</td>
					</tr>
					<tr v-for="i in arr">
						<td>{{i.id}}</td>
						<td>{{i.tit}}</td>
						<td>{{i.con}}</td>
					</tr>
				</table>
			</div>
		</div>

	</div>
</template>

<script>
	export default {
		data() {
			return {
				arr: []
			}
		},
		created() {
			this.$http.get('http://localhost:8000')
				.then((e) => this.arr = e.body)
		}

	}
</script>
<style>
	#box {
		width: 500px;
		height: 300px;
		border: 1px solid #2C3E50;
	}
</style>