<template>
    <div class="todoItem">
        <input v-model="todoItem">
        <button v-on:click="addTodo">Add Todo</button>
        <ul v-for="(todo, index) in todoArray" v-bind:key="index">
            <li v-on:click="removeTodo">
                {{ todo }}
            </li>
            <button v-if="todo">Display Conditionally</button>
        </ul>
    </div>
</template>
<script>
export default {
    name: 'todoAppComponent',
    data() {
        return { todoItem: '', todoArray: [] }
    },
    methods: {
        addTodo() {
            this.todoArray.push(this.todoItem);
        },
        removeTodo() {
            this.todoArray.pop(this.todoItem)
        }
    },
    created() {

    },
    mounted() {
        console.log('mounted lifecycle hook called...')
    }
}
</script>

<style scoped>

</style>