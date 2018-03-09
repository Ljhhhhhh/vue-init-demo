<template>
    <div>
        <ol>
            <li v-for="todo in todos" :key="todo.text">
                {{ todo.text }}
            </li>
        </ol>
        <button @click="eClick()">事件</button>
    </div>
</template>

<script>
export default {
  name: 'indexP',
  data () {
    return {
       todos: [
          { text: 'Learn JavaScript' },
          { text: 'Learn Vue' },
          { text: 'Build something awesome' }
        ]
    }
  },
  methods:{
    eClick(){
        alert('don\'t touch me!')
    }
  }
}
</script>