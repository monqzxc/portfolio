<template>
  <div class="flex flex-col">
    <div
      class="divide-solid divide w-full flex items-center gap-6 flex-row p-2 px-10 m font-bold"
    >
      <div class="flex flex-auto items-center"></div>

      <div v-for="h in header">
        <NavHeader :title="h.title" :link="h.link" />
      </div>
    </div>
    <div class="p-40 flex flex-row w-full items-center gap-64">
      <img
        class="w-auto rounded-full shadow-2xl bg-gray-50"
        src="/resources/images/mon2.jpg"
        style="width: 50vh; height: 50vh"
      />

      <div class="flex flex-col items-center">
        <div class="gap-6 flex flex-col p-4 mr-auto">
          <h1 class="text-5xl font-bold uppercase">Hi there!</h1>
          <h1 class="text-5xl font-bold uppercase">
            I'm Anthony <span class="text-yellow-500">Cabigayan</span>
          </h1>
          <p class="font-bold text-fuchsia-800">Back-end Developer</p>
        </div>
      </div>
    </div>
  </div>
  <div>
    <NuxtPage />
  </div>
</template>
<script>
import NavHeader from "./components/NavHeader.vue";
export default {
  components: {
    NavHeader,
  },
  data() {
    return {
      header: [
        { link: "/about", title: "About" },
        { link: "/skills", title: "Skills" },
        { link: "/projects", title: "Projects" },
        { link: "/experience", title: "Experience" },
      ],
    };
  },
};
</script>
