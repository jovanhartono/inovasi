<script setup>
import { CheckIcon, PhoneIcon, MailIcon } from "lucide-vue-next";
import { RouterView } from "vue-router";
const currentYear = new Date().getFullYear();
</script>

<template>
  <header class="bg-white sticky top-0 z-50">
    <div class="flex items-center justify-between container h-20">
      <a href="#" draggable="false">
        <img
          src="https://12qvr1x1z8.ufs.sh/f/EqFVW2esDyLuX4F4nFyjYV6kKIUpeHhDbnd1RzO925Jxqi0g"
          alt="trademark logo"
          class="size-10"
          loading="eager"
          fetchpriority="high"
          decoding="async"
          draggable="false"
        />
      </a>

      <nav>
        <a
        href="#contact"
          class="rounded-4xl bg-[#1d4762] px-4 h-10 inline-flex items-center text-white relative"
        >
          Get in touch
      </a>
      </nav>
    </div>
  </header>

  <RouterView />

  <footer class="bg-primary text-white" id="contact">
    <div class="flex flex-col sm:flex-row py-12 container gap-6">
      <div class="flex flex-col basis-3/5 shrink-0 max-w-3xl gap-6">
        <h2 class="text-white font-normal">
          <strong class="text-opacity-100"
            > Connect with Us,</strong
          >
          <span class="opacity-70"> for Tailored Solutions and Expert Guidance</span>
        </h2>
        <div class="flex gap-6">
          <div class="flex items-center gap-2">
            <div
              class="shrink-0 size-5 flex items-center justify-center rounded-full text-primary bg-white"
            >
              <CheckIcon class="size-3.5" />
            </div>
            Experienced for more than 10 years
          </div>
          <div class="flex items-center gap-2">
            <div
              class="shrink-0 size-5 flex items-center justify-center rounded-full text-primary bg-white"
            >
              <CheckIcon class="size-3.5" />
            </div>
            Support for the latest technology
          </div>
        </div>

        <div class="flex flex-col gap-2">
            <a class="flex items-center gap-x-2 text-left" href="tel:02178342780">
              <PhoneIcon class="size-4 text-white" />
              <span class="font-medium hover:underline">
                021-7834-2780 
                </span>
            </a>
            <a
              class="flex items-center gap-x-2 text-left"
              href="mailto:inovasi118@gmail.com"
            >
              <MailIcon class="size-4 text-white" />
              <span class="font-medium hover:underline">inovasi118@gmail.com</span>
            </a>
          </div>
      </div>

      <div class="flex justify-end grow items-center">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3965.8301669419473!2d106.80962160549706!3d-6.290545955850148!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f1fa5b9f59a3%3A0x772f6f7bc1fbc6c0!2sMenara%20165!5e0!3m2!1sen!2sid!4v1740321602656!5m2!1sen!2sid"
          class="aspect-square w-full border-0 rounded-xl"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </div>
    </div>

    <div
      class="flex items-center py-6 text-sm text-slate-200 container border-t border-t-slate-500 max-sm:justify-center sm:px-0"
    >
      &copy; {{ currentYear }} PT Inovasi Anugrah Sejahtera. All rights reserved
    </div>
  </footer>
</template>
