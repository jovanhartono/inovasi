<script setup>
import { ShieldCheckIcon } from 'lucide-vue-next'
import { ChartNoAxesColumnIncreasing } from 'lucide-vue-next'
import { PenIcon } from 'lucide-vue-next'
import { InfinityIcon } from 'lucide-vue-next'
import { DatabaseIcon } from 'lucide-vue-next'
import { Layers3Icon } from 'lucide-vue-next'

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
      <div
        class="relative h-[500px] w-full max-sm:flex max-sm:flex-col max-sm:items-center sm:h-[550px]"
      >
        <div class="absolute inset-0 z-10 bg-black/55 sm:rounded-4xl" />
        <img
          src="/batik-bg.webp"
          alt="batik background"
          class="absolute inset-0 z-0 h-[500px] w-full object-cover object-center sm:h-[550px] sm:rounded-4xl"
        />

        <div
          class="relative z-30 flex w-full max-w-5xl flex-col justify-center px-4 max-sm:pt-24 sm:h-full sm:px-16"
        >
          <p class="tracking-wide text-slate-100">#1 General trading company in Indonesia</p>
          <h1 class="text-balance text-white">Delivering Excellence Across Industries</h1>
        </div>

        <div
          class="z-30 h-1/5 w-full max-w-sm rounded-4xl bg-white/5 px-8 py-4 text-white backdrop-blur-xs max-sm:mt-12 sm:absolute sm:right-16 sm:bottom-8 sm:max-w-lg"
        >
          <dl
            class="grid h-full grid-cols-3 items-start gap-4 [&_dd]:text-sm [&_dd]:text-balance [&_dd]:opacity-80 [&_dt]:text-3xl [&_dt]:sm:text-4xl"
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
    <section class="container flex flex-col gap-4 py-8 sm:gap-12 sm:py-16">
      <div class="flex flex-col items-center gap-4 *:flex-1 sm:flex-row">
        <h2 class="text-balance sm:text-center">
          Focusing on Quality,
          <span class="font-normal text-slate-500">we maintain customer trust</span>
        </h2>
        <p>
          PT Inovasi Anugerah Sejahtera menyediakan layanan investasi logam mulia yang dapat menjadi
          alternatif investasi yang aman ditengah pasar yang fluktuatif. Dengan sistem transaksi
          yang transparan dan harga yang kompetitif, perusahaan ini memberikan kemudahan bagi para
          investor yang ingin menambah portofolio investasi mereka dalam bentuk logam mulia dengan
          nilai jangka panjang.
        </p>
      </div>

      <div class="relative h-[500px]">
        <img
          src="https://12qvr1x1z8.ufs.sh/f/EqFVW2esDyLuZcyE8BUyAK1blzsP2o9Cm7TGgIwexSMkqBjR"
          alt=""
          class="h-full w-full rounded-4xl object-cover object-center"
        />
        <div class="bg-primary/30 absolute inset-0 z-10 rounded-4xl" />
      </div>
    </section>

    <!-- Software or AI -->
    <section class="flex flex-col gap-8 bg-slate-100 px-4 py-16 sm:gap-16">
      <div class="flex flex-col">
        <h2 class="mx-auto text-center text-balance">
          <strong class="font-medium">Innovative Consulting,<br /> </strong>
          <span class="font-normal text-slate-500"> for Scalable and Secure Software </span>
        </h2>
        <p class="mt-2 text-center text-balance">
          Menghadirkan solusi piranti lunak berkualitas untuk sektor komersial, industri,
          manufaktur, dan distribusi. Didukung tenaga ahli berpengalaman, kami merancang sistem yang
          efektif, efisien, dan tepat guna guna mendukung operasional bisnis di era digital.
        </p>
      </div>

      <dl
        class="container grid grid-cols-1 overflow-hidden rounded-4xl bg-white px-0 shadow-xs sm:grid-cols-3"
      >
        <div
          v-for="({ title, icon, description }, index) in softwarePoints"
          :key="index"
          class="-mr-px -mb-px border-r border-b px-6 py-10"
        >
          <div class="flex aspect-square size-10 items-center justify-center rounded-md p-2 shadow">
            <component :is="icon" class="text-primary size-5" />
          </div>
          <dt class="text-primary mt-6 text-2xl font-medium tracking-tight">
            {{ title }}
          </dt>
          <dd class="mt-1.5 text-slate-600">
            {{ description }}
          </dd>
        </div>
      </dl>
    </section>

    <section class="py-12 max-sm:px-4">
      <div
        class="z-10 container -mt-24 flex flex-col gap-6 overflow-hidden rounded-4xl bg-white p-6 shadow-sm sm:-mt-20 sm:flex-row"
      >
        <img
          src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scP7ZArIBFL2b4tR1G3W6FmzliNYhXBjDQyK09o"
          alt="property"
          class="aspect-square rounded-xl object-cover sm:w-1/2"
        />

        <div class="flex flex-col gap-6 text-balance">
          <h2>A Trusted Advisor for Strategic Real Estate Investments</h2>
          <p>
            Di sektor properti, PT Inovasi Anugerah Sejahtera menawarkan layanan pembelian,
            penjualan dan penyewaan properti komersial dan industri, seperti gedung perkantoran,
            hotel & apartemen, fasilitas pabrik, serta ruang gudang. Perusahaan ini memahami
            pentingnya lokasi yang strategis, harga yang kompetitif dan kualitas properti yang
            terbaik guna mendukung kelancaran operasional bisnis. Dengan berbagai pilihan properti
            yang dapat disesuaikan dengan kebutuhan usaha, PT Inovasi Anugerah Sejahtera memastikan
            setiap klien mendapatkan solusi properti yang terbaik, tepat dan efisien.
          </p>
        </div>
      </div>
    </section>
  </main>
</template>
