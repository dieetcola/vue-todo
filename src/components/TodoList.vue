<script lang="ts" setup>
import { ref, computed, onMounted } from "vue";
import type { Ref } from "vue";
import ListItemPicker from "./ListItemPicker.vue";
</script>

<template>
  <ListItemPicker />
</template>

<style scoped>
ul {
  list-style: none;
}

li {
  margin: 0.4rem 0;
}
</style>
