<template>
  <div class="flex flex-row flex-wrap justify-evenly sm:flex-row">
    <div v-for="project in projects" :key="project.title" class="w-full sm:w-max sm:max-w-xs md:max-w-sm m-2 p-6 bg-white shadow sm:rounded-lg">
      <div>
        <h3 class="text-xl leading-7 font-semibold border-b border-dashed my-2">
          {{ project.title }}
        </h3>
        <p class="text-gray-700">
          {{ project.description }}
        </p>
      </div>

<!--      <div class="flex flex-row justify-between m-2">
        <NuxtLink :to="{ name: 'consultant-projects-slug', params: { slug: project.slug } }">
        <div
          class="text-center p-2 mt-6 mx-auto bg-transparent font-bold text-blue-500 rounded-md shadow-md hover:bg-blue-400 hover:text-white focus:outline-none focus:bg-blue-400 transition ease-in-out duration-150">
          Read more...
        </div>
        </NuxtLink>
      </div>-->

    </div>

  </div>


</template>
<script lang="ts">
export default {
  name: 'ProjectTiles',
  props: {
    projects: {type: Array, default: () => []}
  }
}
</script>
