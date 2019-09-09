<template>
    <div class="bloglist">
        <h1>My Posts</h1>
        <ul>
            <li v-for="p in blogPosts">{{p.title}}</li>
        </ul>
    </div>
</template>
<script>
export default {
  computed: {
    blogPosts() {
      return this.$store.state.blogPosts;
    },
  },
    
}
</script>