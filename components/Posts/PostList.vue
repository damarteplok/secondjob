<template>
  <div>
    <section class="posts-list">
      <PostPreview
        id="1"
        thumbnail="http://0.soompi.io/wp-content/uploads/2016/03/31204343/twice-tzuyu-2.jpg"
        title="Hello there"
        previewText="This my first post"
      />
      <PostPreview
        id="2"
        thumbnail="http://0.soompi.io/wp-content/uploads/2016/03/31204343/twice-tzuyu-2.jpg"
        title="Hello there2"
        previewText="This my first post2"
      />
      <PostPreview
        id="3"
        thumbnail="http://0.soompi.io/wp-content/uploads/2016/03/31204343/twice-tzuyu-2.jpg"
        title="Hello there3"
        previewText="This my first post3"
      />
      <PostPreview
        id="4"
        thumbnail="http://0.soompi.io/wp-content/uploads/2016/03/31204343/twice-tzuyu-2.jpg"
        title="Hello there4"
        previewText="This my first post4"
      />
    </section>
  </div>
</template>
<script>
import PostPreview from "@/components/Posts/PostPreview";
export default {
  components: {
    PostPreview
  }
};
</script>

<style scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
