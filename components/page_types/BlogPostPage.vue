<template>
  <div>
    <page-title :title="page.name" />
    <div class="relative px-6 sm:px-8 md:px-12">
      <blog-post-meta-data :blog-post="page" class="pt-6" />
    </div>
    <content-blocks :blocks="page.blocks" class="pt-6" />
  </div>
</template>

<script>
import PageTitle from '../PageTitle';
import BlogPostMetaData from '../BlogPostMetaData';
import BlogPostExcerpt from '../BlogPostExcerpt';
import ContentBlocks from '../ContentBlocks';

export default {
  props:['page'],
  components: { 
    PageTitle, BlogPostMetaData, BlogPostExcerpt, ContentBlocks 
  }
}
</script>