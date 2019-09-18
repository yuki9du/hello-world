<template>
    <ul>
        <li v-for="todo in todos" :key="todo.id">
            <slot :wpp="todo"></slot>
            <p>{{todo}}</p>
        </li>
    </ul>
</template>

<script>
export default {
props:{
    todos:{
        type:Array
    }
}
}
</script>

<style>

</style>