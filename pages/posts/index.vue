<template>
  <div class="posts-page">
    <h1>Posts</h1>
    <nuxt-link to="/posts/1">Post 1</nuxt-link>
    <nuxt-link to="/posts/2">Post 2</nuxt-link>
    <nuxt-link to="/posts/3">Post 3</nuxt-link>
  </div>
</template>
<script>

</script>

<style scoped>
.posts-page {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
