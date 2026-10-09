<template>
  <div class="slide-page-layer">
    <div class="slide-page-number">{{ $page }}</div>
  </div>
</template>

<style>
.slide-page-layer {
  position: absolute;
  inset: 0;
  z-index: 50;
  pointer-events: none;
}

.slide-page-number {
  position: absolute;
  top: 20px;
  right: 40px;
  min-width: 32px;
  text-align: right;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 11px;
  line-height: 1;
  font-weight: 400;
  color: var(--muted, #8a8a8a);
}
</style>
