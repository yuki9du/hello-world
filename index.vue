<template>
    <todo-list :todos="todos" class="aaa">
        <span  slot-scope="lyc"> {{lyc.wpp}}</span>
    </todo-list>
</template>

<script>
import todoList from './todoList'
export default {
	components: {
		todoList
	},
	data() {
		return {
			todos: [
				{
					id: 0,
					text: 'ziwei0',
					isComplete: false
				},
				{
					text: 'ziwei1',
					id: 1,
					isComplete: true
				},
				{
					text: 'ziwei2',
					id: 2,
					isComplete: false
				},
				{
					text: 'ziwei3',
					id: 3,
					isComplete: false
				}
			]
		}
	}
}
</script>
<style>
.aaa{
  color: red !important;
}
</style>