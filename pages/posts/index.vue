<template>
  <div class="posts-page">
    <post-list/>
  </div>
</template>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-content: center;
}
</style>
<script>
import PostList from "@/components/Posts/PostList";
export default {
  components: {PostList}
}
</script>
