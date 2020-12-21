<template>
  <button
    @click="foo = 5"
    @focus="doIt(foo)"
  />
</template>

<script lang="ts">
import { defineComponent, ref } from '@vue/composition-api'

export default defineComponent({
  setup: () => ({
    foo: ref(0),
    doIt: (value: number) => console.log(value)
  })
})
</script>
