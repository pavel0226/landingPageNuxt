<template>
  <div data-aos="fade-up" class="sm:col-span-12 md:col-span-6 lg:col-span-4 space-y-6 sm:space-y-3 text-center">
    <img class="rounded-tl-lg rounded-br-lg" :src="require(`~/assets/img/Gallery/${step.img}`)" alt="" />
    <h3 class="text-xl text-white font-semibold">{{ step.title }}</h3>
    <p class="text-sm text-white leading-relaxed">
      {{ step.description }}
    </p>
  </div>
</template>
<script>
export default {
  name: 'LandingStep',
  props: {
    step: {
      type: Object,
      required: true,
    },
  },
}
</script>
