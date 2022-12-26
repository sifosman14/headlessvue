<template>
<article class="col-12 py-5">
  <siv class="card shadow">
    <div class="card-body">
      <h5 class="card-title">
        <NuxtLink :to="{ name: 'slug', params: { slug: post.slug } }">{{ post.title }}</NuxtLink>
      </h5>

      
      <div class="card-text" v-html="post.excerpt"></div>
    </div>
  </siv>
</article>  
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: ['post'],
})
</script>
