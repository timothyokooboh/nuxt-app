<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm 
        :post="loadedPost"
      />
    </section>
    
  </div>
</template>

<script>
import AdminPostForm from '~/components/Admin/AdminPostForm'
export default {
  layout: 'admin',
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: 'Timothy Okooboh',
        title: 'Asynchronous javascript',
        content: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Excepturi animi magni sapiente non, architecto pariatur voluptatum, deleniti harum molestias omnis placeat voluptate perspiciatis maiores doloribus vero ut commodi eos? Nostrum.',
        thumbnailLink: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQBXo2OuF-z10ezJrnHent5wx5VR4HaJrDY-53w3zOB0sVzaRVx&usqp=CAU'
      }
    }
  }
}
</script>

<style scoped>
  .update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>