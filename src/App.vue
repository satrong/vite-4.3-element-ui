<script setup>
import { ref } from 'vue'

const count = ref(0)

const list = [
  { name: 'a', age: 1 },
  { name: 'b', age: 2 },
  { name: 'c', age: 3 },
]
</script>

<template>
<div>
  <div>
    <ElButton @click="count++">click</ElButton> <span>{{ count }}</span>
  </div>
  <ElTable :data="list">
    <ElTableColumn label="Name" prop="name"></ElTableColumn>
    <ElTableColumn label="Age" prop="age"></ElTableColumn>
  </ElTable>
</div>
</template>
