<template>

  <Head>
    <Title>TW | BTN Generator</Title>
  </Head>
  <Body class="overflow-x-hidden">

  </Body>


  <div class="absolute inset-0 w-full h-full bg-cover brightness-150 hue-animation" style="background-image:url(/images/bg-3.webp);"/>
  <div class="absolute inset-0 w-full h-full bg-cover brightness-150 hue-animation" style="background-image:url(/images/bg-2.webp);animation-delay: 38s"/>
  <div class="absolute inset-0 w-full h-full bg-cover brightness-150 hue-animation" style="background-image:url(/images/bg-6.webp);animation-delay: 66s"/>

  <a href="https://github.com/showbear86/tailwind-btn" target="_blank" class="inline-flex items-center justify-center w-6 h-6 xl:w-8 xl:h-8 fill-current text-white transition-all duration-200 ease-out hover:text-cyan-500 absolute right-4 top-4">
    <svg xmlns="http://www.w3.org/2000/svg" class="w-full h-full" viewBox="0 0 512 512"><path d="m256 0c-140.609375 0-256 115.390625-256 256 0 119.988281 84.195312 228.984375 196 256v-84.695312c-11.078125 2.425781-21.273438 2.496093-32.550781-.828126-15.128907-4.464843-27.421875-14.542968-36.546875-29.910156-5.816406-9.8125-16.125-20.453125-26.878906-19.671875l-2.636719-29.882812c23.253906-1.992188 43.371093 14.167969 55.3125 34.230469 5.304687 8.921874 11.410156 14.152343 19.246093 16.464843 7.574219 2.230469 15.707032 1.160157 25.183594-2.1875 2.378906-18.972656 11.070313-26.074219 17.636719-36.074219v-.015624c-66.679687-9.945313-93.253906-45.320313-103.800781-73.242188-13.976563-37.074219-6.476563-83.390625 18.238281-112.660156.480469-.570313 1.347656-2.0625 1.011719-3.105469-11.332032-34.230469 2.476562-62.546875 2.984375-65.550781 13.078125 3.867187 15.203125-3.890625 56.808593 21.386718l7.191407 4.320313c3.007812 1.792969 2.0625.769531 5.070312.542969 17.371094-4.71875 35.683594-7.324219 53.726563-7.558594 18.179687.234375 36.375 2.839844 54.464844 7.75l2.328124.234375c-.203124-.03125.632813-.148437 2.035157-.984375 51.972656-31.480469 50.105469-21.191406 64.042969-25.722656.503906 3.007812 14.128906 31.785156 2.917968 65.582031-1.511718 4.65625 45.058594 47.300781 19.246094 115.753906-10.546875 27.933594-37.117188 63.308594-103.796875 73.253907v.015624c8.546875 13.027344 18.816406 19.957032 18.761719 46.832032v105.722656c111.808594-27.015625 196-136.011719 196-256 .003906-140.609375-115.386719-256-255.996094-256zm0 0"/></svg>
  </a>

  <div class="relative flex flex-col justify-start py-12 min-h-screen max-w-[90vw] xl:max-w-[1322px] -translate-x-px w-full mx-auto">
    <h1 class="select-none break-words text-5xl 2xl:text-[5em] flex flex-col xl:flex-row items-center justify-center text-center xl:gap-4 leading-none font-black text-transparent bg-clip-text bg-gradient-to-b from-cyan-300 to-cyan-600 drop-shadow-lg xl:tracking-tighter">
      <svg xmlns="http://www.w3.org/2000/svg" class="hidden xl:block w-10 h-10 fill-current text-cyan-400" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" x="0px" y="0px" viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve">
              <path d="M490.667,405.333h-56.811C424.619,374.592,396.373,352,362.667,352s-61.931,22.592-71.189,53.333H21.333    C9.557,405.333,0,414.891,0,426.667S9.557,448,21.333,448h270.144c9.237,30.741,37.483,53.333,71.189,53.333    s61.931-22.592,71.189-53.333h56.811c11.797,0,21.333-9.557,21.333-21.333S502.464,405.333,490.667,405.333z M362.667,458.667    c-17.643,0-32-14.357-32-32s14.357-32,32-32s32,14.357,32,32S380.309,458.667,362.667,458.667z"/>
        <path d="M490.667,64h-56.811c-9.259-30.741-37.483-53.333-71.189-53.333S300.736,33.259,291.477,64H21.333    C9.557,64,0,73.557,0,85.333s9.557,21.333,21.333,21.333h270.144C300.736,137.408,328.96,160,362.667,160    s61.931-22.592,71.189-53.333h56.811c11.797,0,21.333-9.557,21.333-21.333S502.464,64,490.667,64z M362.667,117.333    c-17.643,0-32-14.357-32-32c0-17.643,14.357-32,32-32s32,14.357,32,32C394.667,102.976,380.309,117.333,362.667,117.333z"/>
        <path d="M490.667,234.667H220.523c-9.259-30.741-37.483-53.333-71.189-53.333s-61.931,22.592-71.189,53.333H21.333    C9.557,234.667,0,244.224,0,256c0,11.776,9.557,21.333,21.333,21.333h56.811c9.259,30.741,37.483,53.333,71.189,53.333    s61.931-22.592,71.189-53.333h270.144c11.797,0,21.333-9.557,21.333-21.333C512,244.224,502.464,234.667,490.667,234.667z     M149.333,288c-17.643,0-32-14.357-32-32s14.357-32,32-32c17.643,0,32,14.357,32,32S166.976,288,149.333,288z"/>
              </svg>
      <span class="select-none inline-block bg-gradient-to-bl text-transparent bg-clip-text from-cyan-400 to-cyan-600">TW-BUTTON</span>
      <span>GENERATOR</span>
      <svg xmlns="http://www.w3.org/2000/svg" class="hidden xl:block w-10 h-10 fill-current text-cyan-400" height="512" viewBox="0 0 64 64" width="512"><path d="m33 45.5v13.5c0 .54999-.45001 1-1 1h-3.73999c-1.24571.00294-2.31355-.92851-2.47003-2.16004-.29538-1.67221-1.43713-3.07796-3.02997-3.69001-1.54999-.63995-3.32001-.44-4.69001.54004-.97285.72762-2.34996.62338-3.22998-.25 0 0-5.28003-5.28003-5.28003-5.28003-.85091-.83309-.97953-2.27032-.25999-3.21997 2.13107-2.7872.25989-7.24569-3.16014-7.73992-1.22522-.14379-2.14133-1.23137-2.13987-2.46007 0-.00001 0-7.47999 0-7.47999-.00212-1.22831.9151-2.30702 2.14001-2.46004 2.29891-.38963 4.08957-2.52106 4.06999-4.88.00002-1.02995-.31999-2.02-.92002-2.86998-.70996-.97998-.59998-2.33002.27002-3.21002 0 0 5.28003-5.27997 5.28003-5.27997.84998-.84003 2.25995-.96002 3.21997-.26001 2.78622 2.13746 7.33111.24738 7.73993-3.21015.20007-1.20983 1.24005-2.08984 2.46008-2.08984h3.73999c.54999 0 1 .45001 1 1v13.5c0 .54999-.45001 1-1 1-16.58935.69377-16.57076 24.31513.00009 25.00002.54989-.00002.99991.44999.99991.99998z"/><path d="m53.90998 47.83996c-.19627 6.1575-9.12414 6.1589-9.31995-.0001 0-.91988.27997-1.76986.75-2.4999l-5.04004-5.02997h-7.29999c-.54999 0-1-.44-1-1 0-.54999.45001-1 1-1h7.71997c.26001 0 .52002.10999.71002.29999l5.32001 5.32001c2.92636-2.01788 7.26869.33482 7.15997 3.90997z"/><path d="m60 32c-.11875 5.56528-7.92346 6.36791-9.20001.9999 0 .0001-17.79999.0001-17.79999.0001-1.30469-.02249-1.32085-1.9741.00005-2-.00005 0 17.79994 0 17.79994 0 1.27213-5.36727 9.0862-4.56363 9.20001 1z"/><path d="m40.29999 23.69 5.04004-5.03003c-2.03308-2.9341.32311-7.26506 3.91007-7.15988 6.1504.19524 6.1647 9.11146-.0002 9.30991-.91988 0-1.77993-.27002-2.4999-.73999l-5.32001 5.32001c-.19.18994-.45001.29999-.71002.29999h-7.71997c-1.30828-.02517-1.31843-1.97329.00005-2-.00005 0 7.29994 0 7.29994 0z"/></svg>
    </h1>
    <h2 class="text-white font-bold text-base xl:text-2xl text-center leading-none mt-2 xl:mt-0">Easy and Modern Tailwind CSS - Button Generator <span class="text-xs">v.0.6</span></h2>
    <div class="flex flex-col justify-start gap-4 bg-white p-4 xl:p-12 shadow-xl shadow-gray-950/80 border border-white rounded w-full min-h-[660px] translate-y-[18px]">
      <RangeSlider v-model="padding.values.l" attr-side="pl" :range="padding.range"/>
      <RangeSlider v-model="padding.values.r" attr-side="pr" :range="padding.range"/>
      <RangeSlider v-model="padding.values.t" attr-side="pt" :range="padding.range"/>
      <RangeSlider v-model="padding.values.b" attr-side="pb" :range="padding.range"/>
      <RangeSlider v-model="width.value" attr-side="w" :range="width.range"/>

      <input type="text" v-model="button_text" class="inline-flex self-start border border-gray-300 appearance-none px-4 py-2 rounded-lg shadow-md">

      <button class="bg-cyan-400 text-cyan-900 font-bold rounded-lg shadow-lg shadow-cyan-600/30 self-start border mt-12 transition-all duration-200 ease-out hover:bg-cyan-500 border-cyan-500 hover:border-cyan-600" :class="`w-${width.value} pl-${padding.values.l } pr-${padding.values.r } pt-${padding.values.t } pb-${padding.values.b }`">{{button_text}}</button>
    </div>

    <div class="hidden pl-0 pl-px pl-0.5 pl-1 pl-1.5 pl-2 pl-2.5 pl-3 pl-3.5 pl-4 pl-5 pl-6 pl-7 pl-8 pl-9 pl-10 pl-11 pl-12 pl-14 pl-16 pl-20 pl-24 pl-28 pl-32 pl-36 pl-40 pl-44 pl-48 pl-52 pl-56 pl-60 pl-64 pl-72 pl-80 pl-96 pr-0 pr-px pr-0.5 pr-1 pr-1.5 pr-2 pr-2.5 pr-3 pr-3.5 pr-4 pr-5 pr-6 pr-7 pr-8 pr-9 pr-10 pr-11 pr-12 pr-14 pr-16 pr-20 pr-24 pr-28 pr-32 pr-36 pr-40 pr-44 pr-48 pr-52 pr-56 pr-60 pr-64 pr-72 pr-80 pr-96 pb-0 pb-px pb-0.5 pb-1 pb-1.5 pb-2 pb-2.5 pb-3 pb-3.5 pb-4 pb-5 pb-6 pb-7 pb-8 pb-9 pb-10 pb-11 pb-12 pb-14 pb-16 pb-20 pb-24 pb-28 pb-32 pb-36 pb-40 pb-44 pb-48 pb-52 pb-56 pb-60 pb-64 pb-72 pb-80 pb-96 pt-0 pt-px pt-0.5 pt-1 pt-1.5 pt-2 pt-2.5 pt-3 pt-3.5 pt-4 pt-5 pt-6 pt-7 pt-8 pt-9 pt-10 pt-11 pt-12 pt-14 pt-16 pt-20 pt-24 pt-28 pt-32 pt-36 pt-40 pt-44 pt-48 pt-52 pt-56 pt-60 pt-64 pt-72 pt-80 pt-96"></div>
  </div>
  <div class="w-0 w-px w-0.5 w-1 w-1.5 w-2 w-2.5 w-3 w-3.5 w-4 w-5 w-6 w-7 w-8 w-9 w-10 w-11 w-12 w-14 w-16 w-20 w-24 w-28 w-32 w-36 w-40 w-44 w-48 w-52 w-56 w-60 w-64 w-72 w-80 w-96 w-auto w-1/12 w-2/12 w-3/12 w-4/12 w-5/12 w-6/12 w-7/12 w-8/12 w-9/12 w-10/12 w-11/12 w-full w-screen w-min w-max w-fit"></div>
</template>

<script setup>
import {ref, watch, onMounted} from 'vue';
import RangeSlider from '@/components/RangeSlider';

const button_text = ref('My Awesome Button!')

const padding = ref({
  range: ["0","px","0.5","1","1.5","2","2.5","3","3.5","4","5","6","7","8","9","10","11","12","14","16","20","24","28","32","36","40","44","48","52","56","60","64","72","80","96"],
  values: {
    l: "6",
    r: "6",
    t: "3",
    b: "3",
  }
})
const width = ref({
  range: ["auto","1/12","2/12","3/12","4/12","5/12","6/12","7/12","8/12","9/12","10/12","11/12","full","screen","min","max","fit","0","px","0.5","1","1.5","2","2.5","3","3.5","4","5","6","7","8","9","10","11","12","14","16","20","24","28","32","36","40","44","48","52","56","60","64","72","80","96"],
  value: "auto"
})

onMounted(() => {
  // for (let i = 0; i < width.value.range.length; i++) {
  //     widthClasses.value.push(`w-${width.value.range[i]}`);
  // }
});

</script>
