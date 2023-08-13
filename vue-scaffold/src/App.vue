<template>
	<div>
		<student name="张三" :age="18"></student>
		<hr/>
		<student name="李四" ></student>
	</div>
</template>

<script>
	//引入School组件
	import Student from './components/Student'

	export default {
		name:'App',
		components:{Student},
	}
</script>
