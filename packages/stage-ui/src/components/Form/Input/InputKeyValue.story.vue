<script setup lang="ts">
import { ref } from 'vue'

import InputKeyValue from './InputKeyValue.vue'

const key = ref('')
const value = ref('')
</script>

<template>
  <Story
    title="Input Key Value"
    group="form"
    :layout="{ type: 'grid', width: 600 }"
  >
    <template #controls>
      <ThemeColorsHueControl />
    </template>

    <InputKeyValue
      v-model:property-key="key"
      v-model:property-value="value"
      key-placeholder="Key"
      value-placeholder="Value"
    />
  </Story>
</template>
