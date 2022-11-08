<template>
  <div>
    <section class="intro">
      <h1>TechLand -- All Tech All the Time</h1>
    </section>
    <div class="home-page">
      <section class="featured-posts">
        <PostPreview
          id="1"
          thumbnail="./images/mobo.jpg"
          title="Motherboards"
          previewText="The new rx753 from..."
        />
      </section>
      <section class="featured-posts">
        <PostPreview
          id="2"
          thumbnail="./images/pc.jpg"
          title="Monitors"
          previewText="Buying a 4k monitor buyers..."
        />
      </section>
      <section class="featured-posts">
        <PostPreview
          id="3"
          thumbnail="./images/coding.jpg"
          title="Programming"
          previewText="Nuxt 3.0 has..."
        />
      </section>
    </div>
  </div>
</template>
<script>
import PostPreview from '../components/posts/PostPreview.vue';
export default {
  components: {
    PostPreview,
  },
};
</script>

<style scoped>
* {
  color: rgb(16, 19, 32);
}

.home-page {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  text-align: center;
  font-weight: 900;
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: rgb(16, 19, 32);
  background-color: rgba(97, 221, 99, 0.695);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 0.3rem 0.3rem 0.5rem 0.01rem rgb(177, 177, 177);
  box-sizing: border-box;
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

.post-preview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

a {
  text-decoration: none;
  color: black;
}

@media (min-width: 850px) {
  .post-preview {
    width: 400px;
    margin: 10px;
  }
}

.post-thumbnail {
  width: 100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}

.post-content {
  padding: 10px;
  text-align: center;
}

a:hover .post-content,
a:active .post-content {
  background-color: rgba(125, 225, 126, 0.749);
}
</style>
