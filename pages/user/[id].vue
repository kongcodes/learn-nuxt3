<template>
  <div>
    <h1>用户页</h1>
    <p>用户id：{{ $route.params.id}}</p>
  </div>
</template>

<script setup lang="ts">
  const route = useRoute()
  console.log(route.params)
  console.log(route.query)
</script>