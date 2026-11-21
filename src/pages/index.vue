<script setup lang="ts">
import { GButton, GPopover, GCard } from '@jclong98/goose/components';
</script>

<template>
  <h1>You did it!</h1>
  <p>
    Visit
    <a class="text-blue-500" href="https://goose.jacoblong.dev/" target="_blank" rel="noopener"
      >goose.jacoblong.dev</a
    >
    to read the documentation
  </p>

  <GPopover
    class="ml-1"
    open
    position-area="right span-bottom"
  >
    <template #activator="{ binding }">
      <GButton v-bind="binding"> Open popover </GButton>
    </template>

    <GCard class="border rounded p-4">
      <p>Working <span class="text-goose">goose</span> popover!</p>
    </GCard>
  </GPopover>
</template>
