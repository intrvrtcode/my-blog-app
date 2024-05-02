<script setup>
import SearchField from "../SearchField.vue";
import SelectField from "../SelectField.vue";
import BlogCard from "../BlogCard.vue";
import PaginationBlog from "../PaginationBlog.vue";
</script>

<template>
  <main>
    <div class="hero min-h-screen bg-base-200">
      <div class="hero-content text-center">
        <div class="max-w-md">
          <h1 class="text-5xl font-bold">Hello there</h1>
          <p class="py-6">
            Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda
            excepturi exercitationem quasi. In deleniti eaque aut repudiandae et
            a id nisi.
          </p>
          <button class="btn btn-primary">Get Started</button>
        </div>
      </div>
    </div>

    <section class="grid grid-cols-12 gap-x-8 p-4">
      <div class="col-span-7">
        <SearchField />
      </div>

      <div class="col-span-5">
        <SelectField />
      </div>
    </section>

    <section class="p-4">
      <BlogCard v-for="num in 3" :key="num" />
    </section>

    <section class="p-4">
      <PaginationBlog />
    </section>
  </main>
</template>
