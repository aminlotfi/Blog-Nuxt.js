<template>
  <section class="post-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://wallpaperaccess.com/full/314785.jpg"
      title="Hello there!"
      previewText="This my first post!" />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://res.cloudinary.com/twenty20/private_images/t_watermark-criss-cross-10/v1540505787000/photosp/a8ced7e9-1d01-46c1-b0f8-f716d88074ca/stock-photo-technology-screen-background-computer-data-code-programming-coding-software-a8ced7e9-1d01-46c1-b0f8-f716d88074ca.jpg"
      title="Hello there - the second time!"
      previewText="This my second post!" />
  </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>


<style scoped>

.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>

