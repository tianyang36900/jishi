<template>
	<div id="app">
		<!--<img src="./assets/logo.png">-->
		<Abc />
		<!--<Sa/>-->
		<!--<HelloWorld msg="Welcome to beijing" />-->
	</div>
</template>

<script>
	//	import Sa from './components/HelloWorld.vue'
	//	import Title from './components/Title.vue'
	//	import Dianji from './components/Dianji.vue'
	//	import Xuanxiangka from './components/Xuanxiangka.vue'
	//	import Xuanxiangka1 from './components/Xuanxiangka1.vue'
//		import Xinwenzixun from './components/Xinwenzixun.vue'
//	import News from './components/News.vue'
import Mysql from './components/Mysql.vue'
	//	import Xialacaidan from './components/Xialacaidan.vue'
	export default {
		name: 'app',
		components: {
			//			Abc: Title,
			//			Abc: Dianji,
			//			Abc: Xuanxiangka,
			//			Abc: Xuanxiangka1,
			//			Abc: Xinwenzixun,
//			Abc: news,
				Abc:Mysql,
			//			Sa
		}
	}
</script>

<style>
	#app {
		font-family: 'Avenir', Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		/*text-align: center;*/
		color: #2c3e50;
		/*margin-top: 60px;*/
	}
</style>