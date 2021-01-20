<template>
  <div>
    <h2 v-html="$page.post.title"/>
    <div v-html="$page.post.content" />
  </div>
</template>

<page-query>
query Post ($path: String!) {
   post: post (path: $path) {
    title
    content
    date (format: "D MMMM YYYY")
  }
}
</page-query>

<script>
export default {
    name: 'Post'
};
</script>

<style lang="scss">
</style>