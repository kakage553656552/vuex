<template>
  <div>
    <div>{{$store.state.count}}</div>
    <button @click="add">add</button>
    <div>{{$store.getters.getTodoById(1)}}</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'hello Kaka'
    }
  },
  methods: {
    add () {
      this.$store.dispatch('increment', 10)
    }
  }
}
</script>
