<script setup>
import { CheckIcon, PhoneIcon, MailIcon } from 'lucide-vue-next'
import { RouterView } from 'vue-router'
const currentYear = new Date().getFullYear()
</script>

<template>
  <header class="sticky top-0 z-50 bg-white">
    <div class="container flex h-20 items-center justify-between">
      <a href="#" draggable="false" class="flex items-center">
        <img
          src="https://12qvr1x1z8.ufs.sh/f/EqFVW2esDyLuX4F4nFyjYV6kKIUpeHhDbnd1RzO925Jxqi0g"
          alt="trademark logo"
          class="size-10"
          loading="eager"
          fetchpriority="high"
          decoding="async"
          draggable="false"
        />
        <img
          src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPwL7ZN0QFEsJcpuf8glRynTvrCUaOLM4XzhBK"
          alt="inovasi wordmark"
          class="-ml-3 h-20"
          loading="eager"
          fetchpriority="high"
          decoding="async"
          draggable="false"
        />
      </a>

      <nav>
        <a
          href="#contact"
          class="relative inline-flex h-10 items-center rounded-4xl bg-[#1d4762] px-4 text-white"
        >
          Get in touch
        </a>
      </nav>
    </div>
  </header>

  <RouterView />

  <footer class="bg-primary text-white" id="contact">
    <div class="container flex flex-col gap-6 py-12 sm:flex-row">
      <div class="flex max-w-3xl shrink-0 basis-3/5 flex-col gap-6">
        <h2 class="font-normal text-white">
          <strong class="text-opacity-100">Connect with Us,</strong>
          <span class="opacity-70"> for Tailored Solutions and Expert Guidance</span>
        </h2>
        <div class="flex gap-6">
          <div class="flex items-center gap-2">
            <div
              class="text-primary flex size-5 shrink-0 items-center justify-center rounded-full bg-white"
            >
              <CheckIcon class="size-3.5" />
            </div>
            Experienced for more than 10 years
          </div>
          <div class="flex items-center gap-2">
            <div
              class="text-primary flex size-5 shrink-0 items-center justify-center rounded-full bg-white"
            >
              <CheckIcon class="size-3.5" />
            </div>
            Support for the latest technology
          </div>
        </div>

        <div class="flex flex-col gap-2">
          <a class="flex items-center gap-x-2 text-left" href="tel:02178342780">
            <PhoneIcon class="size-4 text-white" />
            <span class="font-medium hover:underline"> 021-7834-2780 </span>
          </a>
          <a class="flex items-center gap-x-2 text-left" href="mailto:inovasi118@gmail.com">
            <MailIcon class="size-4 text-white" />
            <span class="font-medium hover:underline">inovasi118@gmail.com</span>
          </a>
        </div>
      </div>

      <div class="flex grow items-center justify-end">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3965.8301669419473!2d106.80962160549706!3d-6.290545955850148!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f1fa5b9f59a3%3A0x772f6f7bc1fbc6c0!2sMenara%20165!5e0!3m2!1sen!2sid!4v1740321602656!5m2!1sen!2sid"
          class="aspect-square w-full rounded-xl border-0"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </div>
    </div>

    <div
      class="container flex items-center border-t border-t-slate-500 py-6 text-sm text-slate-200 max-sm:justify-center sm:px-0"
    >
      &copy; {{ currentYear }} PT Inovasi Anugrah Sejahtera. All rights reserved
    </div>
  </footer>
</template>
