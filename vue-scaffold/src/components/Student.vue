<template>
	<div>
		<h1>{{ msg }}</h1>
		<h2>学生姓名: {{name}}</h2>
		<h2>学生年龄：{{myAge}}</h2>
		<button @click="ageAdd">点我年龄加1</button>
	</div>
</template>

<script>
	export default {
		name:'Student',
		// props: ['name', 'age'],
		// props: {
		// 	name: String,
		// 	age: Number
		// },
		props: {
			name: {
				type: String,
				required: true
			},
			age: {
				type: Number,
				default: 22
			}
		},
		data(){
			return {
				msg:'我是一个学生',
				myAge: this.age
			}
		},
		methods: {
			ageAdd(){
				this.myAge++
			}
		},
	
	}
</script>
