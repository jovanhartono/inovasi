<script setup>
import { Layers3Icon } from "lucide-vue-next";
</script>

<template>
  <main>
    <!-- Hero -->
    <section class="md:container">
      <div class="relative w-full aspect-[2/1]">
        <div class="absolute inset-0 bg-black/55 rounded-4xl z-10" />
        <img
          src="/batik-bg.webp"
          alt="batik background"
          class="w-full object-cover object-center aspect-[2/1] rounded-4xl absolute inset-0 z-0"
        />

        <div
          class="flex flex-col w-full max-w-5xl h-full px-16 justify-center z-30 relative"
        >
          <p class="tracking-wide text-slate-100">
            #1 General trading company in Indonesia
          </p>
          <h1 class="text-balance text-white">
            Delivering Excellence Across Industries
          </h1>
        </div>

        <div
          class="absolute bottom-8 right-16 rounded-4xl bg-white/5 py-4 px-8 backdrop-blur-xs w-full max-w-lg h-1/5 z-30 text-white"
        >
          <dl
            class="grid grid-cols-3 gap-4 [&_dt]:text-4xl [&_dd]:text-sm [&_dd]:opacity-80 [&_dd]:text-balance h-full items-center"
          >
            <div class="flex flex-col gap-1.5">
              <dt>6jt</dt>
              <dd>The company's annual net income</dd>
            </div>
            <div class="flex flex-col gap-1.5">
              <dt>500+</dt>
              <dd>Projects completed worldwide</dd>
            </div>
            <div class="flex flex-col gap-1.5">
              <dt>10rb+</dt>
              <dd>Satisfied customers worldwide</dd>
            </div>
          </dl>
        </div>
      </div>
    </section>

    <!-- Metal Trading -->
    <section class="flex flex-col container gap-12 py-16">
      <div class="flex items-center gap-4 *:flex-1">
        <h2 class="text-balance text-center">
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

      <div class="grid grid-cols-5 gap-8 w-full">
        <div
          v-for="n in 5"
          :key="n"
          class="bg-slate-100 rounded-full p-4 aspect-square flex items-center justify-center"
        >
          <img
            draggable="false"
            src="/gold-ore.png"
            alt="metal trading"
            class="w-1/2 aspect-square object-cover object-center"
          />
        </div>
      </div>
    </section>

    <!-- Software or AI -->
    <section class="py-16 bg-slate-100 flex flex-col gap-16 px-4">
      <h2 class="text-center text-balance max-w-xl mx-auto">
        <strong class="font-medium">We offer quality,</strong>
        <span class="text-slate-500 font-normal">
          with the best materials and service
        </span>
      </h2>

      <dl
        class="grid grid-cols-3 container px-0 bg-white rounded-4xl shadow-xs overflow-hidden"
      >
        <div v-for="n in 6" class="py-10 px-6 border-r border-b -mr-px -mb-px">
          <div
            class="p-2 shadow rounded-md flex items-center justify-center aspect-square size-10"
          >
            <Layers3Icon class="text-primary size-5" />
          </div>
          <dt class="text-2xl tracking-tight mt-6 text-primary font-medium">
            Layered Security
          </dt>
          <dd class="text-slate-600 mt-1.5">
            with layered security, we ensured the safety of every unit we
            provided
          </dd>
        </div>
      </dl>
    </section>

    <section class="py-12">
      <div
        class="flex rounded-4xl -mt-20 bg-white shadow-sm overflow-hidden z-10 container p-6 gap-6">
        <img src='https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scP7ZArIBFL2b4tR1G3W6FmzliNYhXBjDQyK09o' alt="property" class=" object-cover w-1/2 aspect-square rounded-xl" />

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
