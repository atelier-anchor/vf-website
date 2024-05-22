<template>
  <div
    class="border-2 border-light bg-white p-4 text-light transition-colors dark:bg-dark dark:text-light"
  >
    <div class="flex flex-col items-start gap-4">
      <div>
        <LocaleToggler />
        <ColorToggler />
      </div>
      <a
        href="https://atelier-anchor.com"
        target="_blank"
        class="overflow-hidden after:invisible after:block after:h-0 after:font-bold after:content-[attr(data-title)]"
        :data-title="$t('header.visit-atelier-anchor')"
      >
        {{ $t('header.visit-atelier-anchor') }}
      </a>
    </div>
  </div>
</template>

<script setup lang="ts">
import ColorToggler from '@/components/header/ColorToggler.vue'
import LocaleToggler from '@/components/header/LocaleToggler.vue'
</script>
