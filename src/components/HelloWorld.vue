<template>
	<div class="hello">
		<h1>{{ msg }}</h1>
		<el-row class="mb-4">
			<el-button>Default</el-button>
			<el-button type="primary">Primary</el-button>
			<el-button type="success">Success</el-button>
			<el-button type="info">Info</el-button>
			<el-button type="warning">Warning</el-button>
			<el-button type="danger">Danger</el-button>
		</el-row>

		<el-icon :size="size" :color="color">
			<Edit />
		</el-icon>
		<Edit />
	</div>
</template>

<script>
	export default {
		name: 'HelloWorld',
		props: {
			msg: String
		}
	}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	h3 {
		margin: 40px 0 0;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	li {
		display: inline-block;
		margin: 0 10px;
	}

	a {
		color: #42b983;
	}
</style>
