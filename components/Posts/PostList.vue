<template>
  <section class="post-list">
      <PostPreview 
        id="1"
        :is-admin="isAdmin"
        thumbnail="https://cfamedia.ng/wp-content/uploads/2020/01/tech-opportunities.jpeg"
        title="Javascript closures"
        previewText="Closures are functions that are passed as arguments to other functions"
      />
      <PostPreview 
        id="2"
        :is-admin="isAdmin"
        thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQhjdgi1vHE3imj4uYzGVr3aN_NX6QYPNXNRU5EwyQWZb4TkLBg&usqp=CAU"
        title="Collaborating on Github"
        previewText="Closures are functions that are passed as arguments to other functions"
      />
      <PostPreview 
        :is-admin="isAdmin"
        id="3"
        thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQBXo2OuF-z10ezJrnHent5wx5VR4HaJrDY-53w3zOB0sVzaRVx&usqp=CAU"
        title="High order functions"
        previewText="Closures are functions that are passed as arguments to other functions"
      />

    </section>

</template>

<script>

import PostPreview from '~/components/Posts/PostPreview'
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