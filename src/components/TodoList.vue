<script lang="ts" setup>
import ListItem from "./ListItem.vue";

type Item = {
  title: string;
  checked?: boolean;
};

const listItems: Item[] = [
  { title: "Make a todo list app", checked: true },
  { title: "Predict the weather", checked: false },
  { title: "Play some tunes", checked: false },
  { title: "Let's get cooking", checked: false },
  { title: "Pump some iron", checked: false },
  { title: "Track my expenses", checked: false },
  { title: "Organize a game night", checked: false },
  { title: "Learn a new language", checked: false },
  { title: "Publish my work" },
];
</script>

<template>
  <ul>
    <!-- as i understand, if we want pass boolean to props, 
  must use this syntax, otherwise props should be a string
    -->
    <li v-for="(item, key) in listItems" :key="key">
      <ListItem :is-checked="false">This is the slotted content</ListItem>
    </li>
  </ul>
</template>

<style scoped>
ul {
  list-style: none;
}
li {
  margin: 0.4rem 0;
}
</style>
