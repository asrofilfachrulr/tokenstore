<template>
  <div id="card" class="min-w-[100px] min-h-[100px]">
    <slot></slot>
  </div>
</template>

<style scoped>
#card {
  background: var(--bg-overlay-black);
  border: 1px solid var(--bdr-gray);
  border-radius: .5rem;
  padding: 1rem;
}
</style>