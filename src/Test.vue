<template>
  <span v-if="!onSelect">Not selectable</span>
  <span v-else>Selectable</span>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import type { PropType } from 'vue'

type OnSelectCallback = () => void

export default defineComponent({
  props: {
    onSelect: {
      // error here, but only when the type is marked nullable:
      type: Function as PropType<OnSelectCallback | null>,
      default: null
    }
  }
})
</script>
