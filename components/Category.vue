<template>
  <div class="w-full px-2 xs:mb-6 md:mb-12 article-card">
    <NuxtLink
      :to="`/blog/category/${category.name}`"
      class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md xxlmax:flex-col"
    >
      <div class="flex flex-col m-4">
        <h4 class="font-semibold">category</h4>

        <p>{{ category.name }}</p>
      </div>
    </NuxtLink>
  </div>
</template>

<script>
export default {
  props: {
    category: {
      type: Object,
      required: true
    }
  }
}
</script>
