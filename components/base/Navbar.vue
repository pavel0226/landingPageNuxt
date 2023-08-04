<template>
  <nav id="navbar" class="relative z-10 w-full text-neutral-800 pt-12 md:pt-8 sm:pt-12">
    <div class="flex flex-col max-w-screen-xl px-8 mx-auto lg:items-center lg:justify-between lg:flex-row py-4">
      <div class="flex flex-col lg:flex-row items-center space-x-4 xl:space-x-8">
        <div class="w-full flex flex-row items-center justify-between py-6">
          <div>
            <img :src="require('~/assets/img/logo/secur.svg')" class="w-24 xl:w-28" alt="Nefa Logo" />
          </div>
          <button class="rounded-lg lg:hidden focus:outline-none focus:shadow-outline text-white hover:text-[#666666]" @click="open = !open">
            <SegmentIcon v-if="!open" :size="24" />
            <CloseIcon v-else :size="24" />
          </button>
        </div>
        <ul
          :class="[open ? 'flex' : 'hidden lg:flex']"
          class="w-full h-auto flex flex-col flex-grow lg:items-center pb-4 lg:pb-0 lg:justify-end lg:flex-row origin-top duration-300 xl:space-x-2 space-y-3 lg:space-y-0"
        >
          <NavLink color="text-white hover:text-[#666666]" name="Advantage" url="#advantage" />
          <NavLink color="text-white hover:text-[#666666]" name="Usage" url="#usage" />
          <NavLink color="text-white hover:text-[#666666]" name="TechSpec" url="#techspec" />
          <NavLink color="text-white hover:text-[#666666]" name="Gallery" url="#gallery" />
          <NavLink color="text-white hover:text-[#666666]" name="Contact" url="#contact" />
        </ul>
      </div>
      <div :class="[open ? 'flex' : 'hidden lg:flex']" class="space-x-3">
        <base-button class="px-8 xl:px-10 py-3 mt-2 bg-inherit text-white border border-white hover:text-[#666666] hover:border-[#666666]">
          info@securwallet.com
        </base-button>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  name: 'BaseNavbar',
  data() {
    return {
      open: false,
      dropdownNavbar: false,
    }
  },
  methods: {
    dropdownToggler () {
      this.dropdownNavbar = !this.dropdownNavbar
    }
  }
}
</script>
