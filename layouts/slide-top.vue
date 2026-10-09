<template>
  <div class="slide-page-number">{{ $page }}</div>
</template>

<style scoped>
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
  color: #8a8a8a;
  z-index: 20;
  pointer-events: none;
}
</style>
