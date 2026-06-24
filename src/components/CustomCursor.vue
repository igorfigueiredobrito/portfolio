<template>
  <div class="cursor-ring" id="cursorRing" aria-hidden="true"></div>
  <div class="cursor-dot" id="cursorDot" aria-hidden="true"></div>
</template>

<script setup>
import { onMounted } from 'vue';

onMounted(() => {
  if (window.matchMedia('(hover: hover) and (pointer: fine)').matches) {
    const dot = document.getElementById('cursorDot');
    const ring = document.getElementById('cursorRing');
    let mx = window.innerWidth/2, my = window.innerHeight/2;
    let rx = mx, ry = my;
    document.body.classList.add('cursor-ready');
    window.addEventListener('mousemove', e => {
      mx = e.clientX; my = e.clientY;
      if(dot) dot.style.transform = `translate(${mx}px, ${my}px) translate(-50%,-50%)`;
    });
    function loop() {
      rx += (mx - rx) * 0.18;
      ry += (my - ry) * 0.18;
      if(ring) ring.style.transform = `translate(${rx}px, ${ry}px) translate(-50%,-50%)`;
      requestAnimationFrame(loop);
    }
    loop();
    document.querySelectorAll('a, button, [data-magnetic], .stack-pill, .channel, .testi-card, .svc-card, .tl-card').forEach(el => {
      el.addEventListener('mouseenter', () => ring?.classList.add('is-link'));
      el.addEventListener('mouseleave', () => ring?.classList.remove('is-link'));
    });
  }
});
</script>
