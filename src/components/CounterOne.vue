<template>
  <h2>Counter: {{counter}}</h2>
</template>

<script>
import { inject } from '@vue/runtime-core'

export default {
    setup(){
        const counter = inject('counter')

        return {counter}
    }
}
</script>
