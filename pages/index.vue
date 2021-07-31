<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news</h1>
    </section>
    <section class="featured-posts">
      <post-preview
        id="1"
        thumbnail="https://wallpaperaccess.com/full/210901.jpg"
        title="Tech 1"
        preview-text="Hi, this is  my first post"
      />
      <post-preview
        id="2"
        thumbnail="https://res.cloudinary.com/twenty20/private_images/t_watermark-criss-cross-10/v1540505787000/photosp/a8ced7e9-1d01-46c1-b0f8-f716d88074ca/stock-photo-technology-screen-background-computer-data-code-programming-coding-software-a8ced7e9-1d01-46c1-b0f8-f716d88074ca.jpg"
        title="Tech 2"
        preview-text="Hi, this is  my second post"
      />
    </section>
  </div>
</template>

<script>
  import PostPreview from '@/components/PostPreview.vue';

export default {
  comments: {
    PostPreview,
  }
}
</script>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url("~assets/images/6.1 main-page-background.jpg");
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
