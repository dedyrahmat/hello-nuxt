<template>
  <div>
    <h1>{{ this.slug }}</h1>
    <p>Path: {{ $route.path }}</p>
    <NuxtLink class="bg-blue-400 px-5 py-3 mx-5 my-3" to="/">back</NuxtLink>
  </div>
</template>
<script>
export default {
  async asyncData({ params }) {
    const slug = params.slug
    return { slug }
  },
}
</script>