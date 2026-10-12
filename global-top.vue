<template>
  <div class="apero-page-number">{{ $nav.currentPage }}</div>
</template>

<style>
.apero-page-number {
  position: absolute;
  top: 26px;
  right: 40px;
  z-index: 100;
  min-width: 32px;
  text-align: right;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  line-height: 1;
  font-weight: 400;
  color: var(--muted, #8a8a8a);
  pointer-events: none;
}
</style>
