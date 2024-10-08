<template>
  <div>
    <h3>{{ title }}</h3>
    <ul>
      <li v-for="todo in todos" :key="todo.id">{{ todo.content }}</li>
    </ul>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

const props = defineProps<{
  title: string;
  active: boolean;
  todos: Array<{ id: number; content: string }>;
}>();
</script>
