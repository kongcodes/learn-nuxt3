<template>
  <div>
    <!-- <Title>关于我们</Title> -->
    <h1>关于我们</h1>
    <!--assets -->
    <img src="~/assets/1.png" alt="">
    <!-- public -->
    <img src="/1.png" alt="">
  </div>
</template>

<script setup lang="ts">
  useHead({
    title: '关于我们-',
    titleTemplate(title) {
        return title ? `xx网站 - ${title}` : 'xx网站'
    },
    meta: [
      { name: 'description', content: '网页的描述'},
      { name: 'keywords', content: '关键字1'},
    ],
    bodyAttrs: {
      class: 'red'
    },
    script: [
      {
        src: 'assets/a.js',
        body: true
      }
    ]
  })
</script>

<style>
  .red {
    color: red;
  }
</style>