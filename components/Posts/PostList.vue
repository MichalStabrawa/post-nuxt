<template>
  <section class="post-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      title="title1"
      thumbnail="https://cdn.pixabay.com/photo/2013/06/09/09/07/explosion-123690_1280.jpg"
      previewText="my post 2"
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      title="title2"
      thumbnail="https://cdn.pixabay.com/photo/2015/03/26/09/43/camera-690163_1280.jpg"
      previewText="my post 3"
    />
    <PostPreview
      id="3"
      :is-admin="isAdmin"
      title="title3"
      thumbnail="https://cdn.pixabay.com/photo/2016/02/19/11/51/world-trade-center-1210003_1280.jpg"
      previewText="my post 1"
    />
  </section>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";
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
};
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

