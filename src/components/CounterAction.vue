<template>
  <button @click="counter++">+</button>
  <button @click="counter--">-</button>
</template>

<script>
import { inject } from '@vue/runtime-core'
export default {
    setup() {
        const counter = inject('counter')

        return {counter}
    }
}
</script>
