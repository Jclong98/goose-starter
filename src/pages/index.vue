<script setup lang="ts">
import { GButton, GPopover } from '@jclong98/goose/components';
</script>

<template>
  <h1>You did it!</h1>
  <p>
    Visit
    <a class="text-blue-500" href="https://goose.jacoblong.dev/" target="_blank" rel="noopener">goose.jacoblong.dev</a> to
    read the documentation
  </p>

  <GPopover class="border border-current/50 ml-1 px-4 py-3 rounded-lg" open position-area="right span-bottom">
    <template #activator="{ binding }">
      <GButton v-bind="binding"> Open popover </GButton>
    </template>

    <p>Working <span class="text-goose">goose</span> popover!</p>
  </GPopover>
</template>
