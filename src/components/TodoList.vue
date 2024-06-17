<script lang="ts" setup>
import ListItem from "./ListItem.vue";
</script>

<template>
  <ul>
    <!-- as i understand, if we want pass boolean to props, 
  must use this syntax, otherwise props should be a string
    -->
    <ListItem :is-checked="false">This is the slotted content</ListItem>
  </ul>
</template>
