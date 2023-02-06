<template>
	<div>
		<el-table ref="" v-bind="dataOptions" style="width: 100%">
			<el-table-column prop="date" label="Date" width="180" />
			<el-table-column prop="name" label="Name" width="180" />
			<el-table-column prop="address" label="Address" />
		</el-table>
		<el-pagination layout="prev, pager, next" :total="1000" />
	</div>
</template>
<script>
	import {
		computed
	} from 'vue'

	export default {
		name: 'JTable2',
		props: {
		},
		setup(props, {
			attrs
		}) {
			const dataOptions = computed(() => {
				console.log("attrs", attrs)
				console.log("prop", props)
				const bindValue = {
					...attrs.dataOptions,
					...attrs,
					...props,
				}
				console.log(bindValue)
				return bindValue

			})
			return {
				dataOptions
			}
		}
	}
</script>

<style>
</style>
