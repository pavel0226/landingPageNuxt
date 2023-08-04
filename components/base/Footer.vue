<template>
  <footer class="max-w-screen-xl px-8 mx-auto">
    <div class="w-full border-t border-[#DDDDDD]">
      <div class="mt-8">
        <a class="my-5" href="#">
          <img :src="require('~/assets/img/logo/secur_origin.svg')" class="w-24 -mt-2" alt="Nefa Logo" />
        </a>
      </div>
      <div class="flex justify-between">
        <ul class="flex flex-row py-8">
          <NavLink name="Advantage" url="#advantage" />
          <NavLink name="Usage" url="#usage" />
          <NavLink name="TechSpec" url="#techspec" />
          <NavLink name="Gallery" url="#gallery" />
        </ul>
        <div class="flex flex-fow py-8">
          <InstagramIcon />
          <TwitterIcon class="mx-4" />
          <FacebookIcon />
        </div>
      </div>
    </div>
    <div class="py-8 sm:py-4 text-center text-sm text-[#666666] hover:text-gray-900">
      &copy; Copyright 2023 SECUR LLC. All rights reserved
    </div>
  </footer>
</template>
<script>
export default {
  name: 'BaseFooter',
}
</script>
