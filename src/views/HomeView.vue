<script setup>
import { ShieldCheckIcon } from "lucide-vue-next";
import { ChartNoAxesColumnIncreasing } from "lucide-vue-next";
import { PenIcon } from "lucide-vue-next";
import { InfinityIcon } from "lucide-vue-next";
import { DatabaseIcon } from "lucide-vue-next";
import { Layers3Icon } from "lucide-vue-next";


const softwarePoints = [
  {
    icon: Layers3Icon,
    title: 'Custom-Built Solutions',
    description: 'Tailored to your business needs for maximum efficiency'
  },
  {
    icon: ShieldCheckIcon,
    title: 'Advanced Security',
    description: 'Enterprise-grade protection against cyber threats'
  },
  {
    icon: PenIcon,
    title: 'Intuitive UX',
    description: 'User-friendly design for seamless operation'
  },
  {
    icon: ChartNoAxesColumnIncreasing,
    title: 'Scalable & Future-Ready',
    description: 'Easily adaptable for business growth'
  },
  {
    icon: InfinityIcon,
    title: 'Ongoing Support',
    description: 'Regular updates and dedicated technical assistance'
  },
  {
    icon: DatabaseIcon,
    title: 'Database Solution',
    description: 'Our expertise spans database design, optimization, migration, and management'
  }
]
</script>

<template>
  <main>
    <!-- Hero -->
    <section class="md:container">
      <div class="relative w-full h-[500px] sm:h-[550px] max-sm:flex max-sm:flex-col max-sm:items-center">
        <div class="absolute inset-0 bg-black/55 sm:rounded-4xl z-10" />
        <img
          src="/batik-bg.webp"
          alt="batik background"
          class="w-full object-cover object-center h-[500px] sm:h-[550px] sm:rounded-4xl absolute inset-0 z-0"
        />

        <div
          class="flex flex-col w-full max-w-5xl max-sm:pt-24 sm:h-full px-4 sm:px-16 justify-center z-30 relative"
        >
          <p class="tracking-wide text-slate-100">
            #1 General trading company in Indonesia
          </p>
          <h1 class="text-balance text-white">
            Delivering Excellence Across Industries
          </h1>
        </div>

        <div
          class="max-sm:mt-12 sm:absolute sm:bottom-8 sm:right-16 rounded-4xl bg-white/5 py-4 px-8 backdrop-blur-xs w-full max-w-sm sm:max-w-lg h-1/5 z-30 text-white"
        >
          <dl
            class="grid grid-cols-3 gap-4 [&_dt]:text-3xl [&_dt]:sm:text-4xl [&_dd]:text-sm [&_dd]:opacity-80 [&_dd]:text-balance h-full items-start"
          >
            <div class="flex flex-col gap-1.5">
              <dt>10B+</dt>
              <dd>AUM</dd>
            </div>
            <div class="flex flex-col gap-1.5">
              <dt>500+</dt>
              <dd>Projects completed</dd>
            </div>
            <div class="flex flex-col gap-1.5">
              <dt>10K+</dt>
              <dd>Satisfied customers</dd>
            </div>
          </dl>
        </div>
      </div>
    </section>

    <!-- Metal Trading -->
    <section class="flex flex-col container gap-4 sm:gap-12 py-8 sm:py-16">
      <div class="flex sm:flex-row flex-col items-center gap-4 *:flex-1">
        <h2 class="text-balance sm:text-center">
          Focusing on Quality,
          <span class="text-slate-500 font-normal"
            >we maintain customer trust</span
          >
        </h2>
        <p>
          PT Inovasi Anugerah Sejahtera menyediakan layanan investasi logam
          mulia yang dapat menjadi alternatif investasi yang aman ditengah pasar
          yang fluktuatif. Dengan sistem transaksi yang transparan dan harga
          yang kompetitif, perusahaan ini memberikan kemudahan bagi para
          investor yang ingin menambah portofolio investasi mereka dalam bentuk
          logam mulia dengan nilai jangka panjang.
        </p>
      </div>

      <div class="relative h-[500px]">
        <img src="https://12qvr1x1z8.ufs.sh/f/EqFVW2esDyLuZcyE8BUyAK1blzsP2o9Cm7TGgIwexSMkqBjR" alt="" class="w-full h-full object-cover object-center rounded-4xl">
        <div class="absolute inset-0 bg-primary/30 rounded-4xl z-10" />
      </div>
    </section>

    <!-- Software or AI -->
    <section class="py-16 bg-slate-100 flex flex-col gap-8 sm:gap-16 px-4">
      <h2 class="text-center text-balance mx-auto">
        <strong class="font-medium">Connect with Us,<br> </strong>
        <span class="text-slate-500 font-normal">
          for tailored solutions and expert guidance
        </span>
        
      </h2>

      <dl
        class="grid grid-cols-1 sm:grid-cols-3 container px-0 bg-white rounded-4xl shadow-xs overflow-hidden"
      >
        <div v-for="{ title, icon, description}, index in softwarePoints" :key="index" class="py-10 px-6 border-r border-b -mr-px -mb-px">
          <div
            class="p-2 shadow rounded-md flex items-center justify-center aspect-square size-10"
          >
            <component :is="icon" class="text-primary size-5" />
          </div>
          <dt class="text-2xl tracking-tight mt-6 text-primary font-medium">
            {{title}}
          </dt>
          <dd class="text-slate-600 mt-1.5">
            {{description}}
          </dd>
        </div>
      </dl>
    </section>

    <section class="py-12 max-sm:px-4">
      <div
        class="flex flex-col sm:flex-row rounded-4xl sm:-mt-20 -mt-24 bg-white shadow-sm overflow-hidden z-10 container p-6 gap-6">
        <img src='https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scP7ZArIBFL2b4tR1G3W6FmzliNYhXBjDQyK09o' alt="property" class="object-cover sm:w-1/2 aspect-square rounded-xl" />

        <div class="flex flex-col gap-6 text-balance">
          <h2 class="text-4xl ">A Trusted Advisor for Strategic Real Estate Investments</h2>
          <p>
            Di sektor properti, PT Inovasi Anugerah Sejahtera menawarkan layanan pembelian, penjualan dan penyewaan properti komersial dan industri, seperti gedung perkantoran, hotel & apartemen, fasilitas pabrik, serta ruang gudang. Perusahaan ini memahami pentingnya lokasi yang strategis, harga yang kompetitif dan kualitas properti yang terbaik guna mendukung kelancaran operasional bisnis. Dengan berbagai pilihan properti yang dapat disesuaikan dengan kebutuhan usaha, PT Inovasi Anugerah Sejahtera memastikan setiap klien mendapatkan solusi properti yang terbaik, tepat dan efisien.
          </p>
        </div>
      </div>
    </section>
  </main>
</template>
