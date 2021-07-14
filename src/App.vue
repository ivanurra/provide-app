<template>
<h1>App Counter: {{counter}}</h1>
<counter-one />
<counter-action/>
</template>

<script>
import { provide, ref } from 'vue'
import CounterOne from './components/CounterOne.vue'
import CounterAction from './components/CounterAction.vue'

export default {
name: 'App',
components: {
    CounterOne,
    CounterAction
},
setup(){
    const counter = ref(0)

    provide('counter', counter)

    return { counter }
}
}
</script>
s
