<template>
    <div>
        
    </div>
</template>

<page-query>
query AllPosts {
    allPosts {
        edges {
            node {
                id
                slug
            }
        }
    }
}
</page-query>

<script>
export default {
    name: 'AllPosts'
}
</script>

<style lang="scss">
    
</style>