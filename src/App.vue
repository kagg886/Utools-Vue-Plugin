<script setup lang="ts">
import {ref} from "vue";

const a = ref<string>()
utools.onPluginEnter((action) => {
  a.value = JSON.stringify(action);
})
</script>

<template>
  {{a}}
</template>

<style scoped>

</style>
