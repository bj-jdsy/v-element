<template>
	<JTable column="abc" :data="dd" :border="false" :show-header="true" :stripe="false" @row-click="bbb"
		:data-options="{data:dd, stripe:true}">
	</JTable>
</template>

<script setup>
	import JTable from './components/table/CTable.vue'
	const bbb = () => {
		console.log('ccc')
	}

	const dd = [{
			date: '2016-05-03',
			name: 'Tom',
			address: 'No. 189, Grove St, Los Angeles',
		},
		{
			date: '2016-05-02',
			name: 'Tom',
			address: 'No. 189, Grove St, Los Angeles',
		},
		{
			date: '2016-05-04',
			name: 'Tom',
			address: 'No. 189, Grove St, Los Angeles',
		},
		{
			date: '2016-05-01',
			name: 'Tom',
			address: 'No. 189, Grove St, Los Angeles',
		},
	]
</script>

<style>

</style>
