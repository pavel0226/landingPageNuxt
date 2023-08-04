<template>
  <div class="w-full">
    <!-- Hero section -->
    <section id="hero" class="w-full pb-24">
      <BaseSection>
        <div class="col-span-12 lg:col-span-6 mt-12 xl:mt-10 space-y-4 sm:space-y-6 px-6 text-center sm:text-left">
          <h1
            data-aos="fade-right"
            data-aos-once="true"
            class="text-[2.5rem] sm:text-5xl xl:text-6xl font-bold leading-tight capitalize sm:pr-8 xl:pr-10"
          >
            <span class="text-header-gradient">Secur Wallet</span>
          </h1>
          <p data-aos="fade-down" data-aos-once="true" data-aos-delay="300" class="hidden sm:block text-white">
            Protect your wallet from unauthorized access.
          </p>
        </div>
        <div class="hidden sm:block col-span-12 lg:col-span-6">
          <div class="w-full">
            <img
              data-aos="fade-up"
              data-aos-once="true"
              :src="require('~/assets/img/case/01.jpg')"
              class="-mt-4"
              alt=""
            />
          </div>
        </div>
        <img
          data-aos="fade-up"
          data-aos-delay="300"
          :src="require('~/assets/img/pattern/ellipse-1.png')"
          class="hidden sm:block absolute bottom-12 xl:bottom-16 left-4 xl:left-0 w-6"
        />
        <img
          data-aos="fade-up"
          data-aos-delay="300"
          :src="require('~/assets/img/pattern/ellipse-2.png')"
          class="hidden sm:block absolute top-4 sm:top-10 right-64 sm:right-96 xl:right-[32rem] w-6"
        />
        <img
          data-aos="fade-up"
          data-aos-delay="300"
          :src="require('~/assets/img/pattern/ellipse-3.png')"
          class="hidden sm:block absolute bottom-56 right-24 w-6"
        />
        <img
          data-aos="fade-up"
          data-aos-delay="300"
          :src="require('~/assets/img/pattern/star.png')"
          class="hidden sm:block absolute top-20 sm:top-28 right-16 lg:right-0 lg:left-[30rem] w-8"
        />
      </BaseSection>
    </section>

    <!-- Crypto statistic section -->
    <section
      class="career px-4 sm:px-6 lg:px-0 py-6 pb-20 sm:py-8 bg-white shadow-lg sm:shadow-md transform lg:-translate-y-12"
    >
      <div class="w-full px-6 sm:px-0 py-16 flex flex-col items-center justify-center space-y-4 text-center">
        <h2 data-aos="flip-down" class="text-2xl text-neutral-800 font-semibold">What exactly is <span class="text-header-gradient">Secur Wallet</span>?</h2>
        <p data-aos="flip-down" class="paragraph max-w-screen-xl">
          Secur Wallet is a smart wallet with 3-digit code lock and tracking system via your smartphone. 
          <br> 
          Now you do not need to be afraid to forget or lose your wallet, as the sound notification system will inform you about this problem. 
          <br> 
          And thanks to the combination lock, no one except you can get quick access to your bank cards and valuables.</p>
      </div>
    </section>

    <!-- Advantage section -->
    <section id="advantage" class="w-full my-24">
      <BaseSection>
        <div data-aos="fade-right" data-aos-delay="150" class="col-span-12 lg:col-span-6">
          <div class="w-full">
            <img :src="require('~/assets/img/case/04.jpg')" class="w-full" alt="" />
          </div>
        </div>
        <div data-aos="fade-left" data-aos-delay="150" class="col-span-12 lg:col-span-6 px-4 sm:px-6 mt-8">
          <h2 class="text-4xl font-semibold">
            Advantages of <span class="text-header-gradient">Secur Wallet</span>
          </h2>
          <ul class="shadow-box mt-3">
            <BaseAccordion v-for="(accordion, index) in advantages" :key="index" :accordion="accordion" />
          </ul>
        </div>
      </BaseSection>
    </section>
    
    <!--How to use section -->
    <section id="usage" class="bg-trading-tools relative max-w-full sm:mx-4 my-20 py-16 shadow rounded-2xl overflow-hidden">
      <div class="relative max-w-screen-xl px-4 sm:px-2 mx-auto grid grid-cols-12 gap-x-6">
        <LandingTradingToolImage class="sm:hidden" />
        <div data-aos="fade-right" class="col-span-12 lg:col-span-6 space-y-8 sm:space-y-6 px-4 sm:px-6 mt-8">
          <h2 class="text-4xl font-semibold">How to use <span class="text-header-gradient">Secur Wallet</span></h2>
          <div class="space-y-4">
            <h4 class="text-lg font-medium">To open the wallet</h4>
            <p class="paragraph text-sm xl:text-base">
              You need to enter the 3-digit opening code on the combination lock and press the sliding button.
            </p>
          </div>
          <div class="space-y-4">
            <h4 class="text-lg font-medium">After closing the wallet</h4>
            <p class="paragraph text-sm xl:text-base">
              You must change the position of the wheels to a random position in order to block the lock mechanism.
            </p>
          </div>
          <div class="space-y-4">
            <h4 class="text-lg font-medium">In order to be able to track the location of your wallet</h4>
            <p class="paragraph text-sm xl:text-base">
              You must download a dedicated Secur wallet management application to your smartphone. The app will prompt you to connect to the wallet using Bluetooth. After establishing a connection with the wallet, you will be able to see its location on the map.
            </p>
          </div>
          <div class="space-y-4">
            <h4 class="text-lg font-medium">Also in the application</h4>
            <p class="paragraph text-sm xl:text-base">
              You have the opportunity to activate the sound notification function when the wallet is lost. If you forget your wallet somewhere and move more than five meters away from it, you will immediately receive an alert on your phone, as well as hear the sound of an alarm coming from your wallet.
            </p>
          </div>
        </div>
        <LandingTradingToolImage data-aos="fade-left" class="hidden sm:block" />
      </div>
    </section>

    <!-- Tech Spec section -->
    <section id="techspec" class="w-full my-24">
      <div class="relative max-w-screen-xl px-8 mx-auto grid grid-cols-12 gap-x-6">
        <div data-aos="fade-right" class="col-span-12 lg:col-span-6">
          <div class="w-full">
            <img :src="require('~/assets/img/case/06.jpg')" class="w-full" alt="" />
          </div>
        </div>
        <div data-aos="fade-left" class="col-span-12 lg:col-span-5 space-y-8 sm:space-y-6 mt-8 xl:px-8">
          <h2 class="text-4xl font-semibold">Technical Specification of <span class="text-header-gradient">Secur Wallet</span></h2>
          <ul class="space-y-8 sm:space-y-4">
            <LandingListItem title="Size 112 x 72 x 18 mm" />
            <LandingListItem title="Capacity up to 8 cards + banknotes" />
            <LandingListItem title="Digital Lock – 1000 code combinations" />
            <LandingListItem title="RFID protection" />
            <LandingListItem title="Audible Alarm" />
            <LandingListItem title="Bluetooth" />
            <LandingListItem title="GPS" />
            <LandingListItem title="Data Storage" />
            <LandingListItem title="USB Type-C" />
          </ul>
        </div>
      </div>
    </section>

    <!-- Gallery section -->
    <section id="gallery" class="bg-black relative max-w-full sm:mx-4 xl:mx-10 my-24 shadow sm:rounded-2xl overflow-hidden">
      <div class="w-full py-16 flex flex-col items-center">
        <h2 data-aos="flip-down" class="text-3xl text-white sm:text-4xl font-semibold text-center">
          Gallery
        </h2>
        <!-- <LandingGallery /> -->
        <div          
          class="grid grid-cols-12 w-full gap-5 px-4 xl:px-10 mt-16 sm:mt-8"
        >
          <LandingStep v-for="step in steps" :key="step.title" :step="step" />
        </div>
      </div>
    </section>

    <!-- Partners section -->
    <section class="bg-partner relative max-w-full sm:mx-6 my-24 shadow sm:rounded-2xl overflow-hidden">
      <div class="w-full px-6 sm:px-0 py-16 flex flex-col items-center justify-center space-y-4 text-center">
        <h3 data-aos="flip-down" class="text-2xl text-neutral-800 font-semibold">Trusted Partners Worldwide</h3>
        <p data-aos="flip-down" class="paragraph">We're partners with countless major organisations around the globe</p>
        <div data-aos="fade-up" class="flex flex-wrap items-center justify-center">
          <LandingPartnerImage
            v-for="img in ['clever.png', 'diamon-cutts.png', 'swiss-finance.png', 'gambio.png']"
            :key="img"
            :img="img"
          />
        </div>
      </div>
    </section>

    <div class="w-full my-10 flex justify-center">
      <a
        v-smooth-scroll
        data-aos="flip-down"
        data-aos-delay="150"
        href="#navbar"
        class="px-6 py-3 flex items-center space-x-2 bg-[#FAFAFA] hover:bg-gray-100 hover:shadow-md border border-[#DDDDDD] rounded-md text-gray-700"
      >
        <span>Back to top</span>
        <ArrowUpIcon :size="20" />
      </a>
    </div>
  </div>
</template>

<script>
import aosMixin from '@/mixins/aos'
export default {
  name: 'IndexPage',
  mixins: [aosMixin],
  data() {
    return {
      selected: 0,
      advantages: [
        {
          title: '3-Digit Code Lock',
          description: "1000 combinations to protect your personal data. Featuring a 3-digit locking code, your belongings are locked away and out of the reach from unauthorized people.",
        },
        {
          title: 'Space for the Most Important Things',
          description: "Holds up to 7 cards + cash. You can safely store your bank cards, ID, driver’s license, insurance, metro cards, SIM cards, cash and more.",
        },
        {
          title: 'Ergonomic Design',
          description: "Secur Wallet has a compact size that allows you to carry it in your pants or jacket pocket. It also fits comfortably in your hand.",
        },
        {
          title: 'Shockproof',
          description: "The wallet is difficult to break or shatter because it has excellent impact resistance characteristics.",
        },
        {
          title: 'RFID Protection',
          description: "Your bank cards will always be protected from being read and demagnetized.",
        },
        {
          title: 'Audible Alarm',
          description: "The sound signal will help you find your wallet and not forget it in the future.",
        },
        {
          title: 'Location Tracking System',
          description: "Track the location of the wallet, being at a considerable distance.",
        },
        {
          title: 'Data Storage',
          description: "Keep the necessary electronic documents and cryptocurrency right in your wallet.",
        },
      ],
      steps: [
        {
          img: '01.jpg',
          title: 'title',
          description: 'here goes some description.',
        },
        {
          img: '02.jpg',
          title: 'title',
          description: 'here goes some description.',
        },
        {
          img: '03.jpg',
          title: 'title',
          description: 'here goes some description.',
        },
        {
          img: '04.jpg',
          title: 'title',
          description: 'here goes some description.',
        },
        {
          img: '05.jpg',
          title: 'title',
          description: 'here goes some description.',
        },
        {
          img: '06.jpg',
          title: 'title',
          description: 'here goes some description.',
        },
      ],
    }
  },
}
</script>
<style scoped>
.career {
  margin-top: -45px;
  margin-left: 15px;
  margin-right: 15px;
  border-radius: 30px;
  background: linear-gradient(341deg, #c8c8c8 -6.01%, #ffffff 36.87%, #e2e5eb 78.04%, #d2d2d2 103.77%);
}
.text-header-gradient {
  background: rgb(57, 132, 244);
  background: linear-gradient(169.4deg, #3984f4 -6.01%, #0cd3ff 36.87%, #2f7cf0 78.04%, #0e65e8 103.77%);
  background-clip: text;
  -webkit-text-fill-color: transparent;
}
.bg-partner {
  background: url('../assets/img/partner/background.png');
  background-size: cover;
  background-position: center;
}
.bg-trading-tools {
  background: linear-gradient(341deg, #c8c8c8 -6.01%, #ffffff 36.87%, #e2e5eb 78.04%, #d2d2d2 103.77%);
  background-size: cover;
  background-position: center;
}
.max-h-0 {
  max-height: 0;
}
</style>
