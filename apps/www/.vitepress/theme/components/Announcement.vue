<script setup lang="ts">
import { Separator } from '@/lib/registry/default/ui/separator'
import ArrowRightIcon from '~icons/radix-icons/arrow-right'
import { announcementConfig } from '../config/site'
</script>

<template>
  <a
    :href="announcementConfig.link"
    class="inline-flex items-center rounded-lg bg-muted px-3 py-1 text-sm font-medium"
  >
    {{ announcementConfig.icon }} <Separator class="mx-2 h-4" orientation="vertical" />
    <span class="sm:hidden">{{ announcementConfig.title }}</span>
    <span class="hidden sm:inline">
      {{ announcementConfig.title }}
    </span>
    <ArrowRightIcon class="ml-1 h-4 w-4" />
  </a>
</template>
