<template>
  <div id="utilitarian_card" class=" sm:w-1/2 m-2 p-6 bg-white overflow-hidden shadow sm:rounded-lg">
    <div class="border-b border-dashed p-4 w-3/5 mx-auto">
      <img :src="logo_path" alt="sideproject_logo">
    </div>
    <div class="my-4 mx-4">
      <slot></slot>

    </div>

  </div>
</template>
<script lang="ts">
export default {
  name: 'SideProjectCard',
  props: ['logo_path']
}
</script>
