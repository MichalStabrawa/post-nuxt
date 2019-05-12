<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news!</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        title="title1"
        thumbnail="https://cdn.pixabay.com/photo/2013/06/09/09/07/explosion-123690_1280.jpg"
        previewText="my post 2"
      />
      <PostPreview
        id="2"
        title="title2"
        thumbnail="https://cdn.pixabay.com/photo/2015/03/26/09/43/camera-690163_1280.jpg"
        previewText="my post 3"
      />
      <PostPreview
        id="3"
        title="title3"
        thumbnail="https://cdn.pixabay.com/photo/2016/02/19/11/51/world-trade-center-1210003_1280.jpg"
        previewText="my post 1"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from "../components/Posts/PostPreview";

export default {
  components: { PostPreview }
};
</script>


<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url("~assets/image/intro.jpg");
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
  background-color: #ccc;
}
</style>




