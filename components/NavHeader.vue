<template>
  <div>
    <div class="ml-auto flex items-center cursor-pointer">
      <NuxtLink :to="link">{{ title }}</NuxtLink>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    title: String,
    link: String,
  },
};
</script>
