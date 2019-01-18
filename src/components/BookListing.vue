<template>
  <div>
    <router-link :to="`/books/${book.id}`"><img :src="book.image" alt="cover image" class="h-64 mb-2"></router-link>
    <router-link :to="`/books/${book.id}`" class="text-lg font-bold text-black hover:text-grey-darkest mb-1 block">
      {{ book.title }}
    </router-link>
    <div class="text-grey-darkest">{{ book.author }}</div>
  </div>
</template>

<script>
export default {
  props: ['book']
}
</script>
