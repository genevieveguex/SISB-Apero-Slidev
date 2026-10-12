<template>
  <div class="slide-page-number">{{ $slidev.nav.currentPage }}</div>
</template>

<style scoped>
.slide-page-number {
  position: absolute;
  right: 40px;
  bottom: 16px;
  z-index: 10;

  color: var(--muted, #666666);
  font-family: Arial, Helvetica, sans-serif;
  font-size: 11px;
  line-height: 1;

  pointer-events: none;
}
</style>
