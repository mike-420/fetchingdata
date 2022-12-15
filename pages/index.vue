<template>
    <ul>
      <li v-for="user in users" :key="user.id">
        {{ user.name }}
      </li>
    </ul>
</template>
<script setup>
  const { data : users } = await useFetch('https://jsonplaceholder.typicode.com/users')
</script>

