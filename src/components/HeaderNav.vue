<template>
  <nav class="nav" id="nav" aria-label="Navegação principal">
    <a href="#home" class="nav-link always active">Início</a>
    <a href="#about" class="nav-link">Sobre</a>
    <a href="#timeline" class="nav-link">Carreira</a>
    <a href="#fisioly" class="nav-link">Fisioly</a>
    <a href="#stack" class="nav-link">Stack</a>
    <a href="#services" class="nav-link">Serviços</a>
    <a href="#contact" class="nav-link">Contato</a>
    <span class="nav-divider" aria-hidden="true"></span>
    <a href="https://api.whatsapp.com/send?phone=5511999999999&text=Ol%C3%A1%2C%20gostaria%20de%20fazer%20um%20or%C3%A7amento!" target="_blank" rel="noopener" class="nav-cta">
      <svg width="13" height="13" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M17.5 14.4c-.3-.1-1.7-.8-2-.9-.3-.1-.5-.1-.7.1-.2.3-.7.9-.9 1.1-.2.2-.3.2-.6.1-.3-.1-1.2-.4-2.3-1.4-.9-.8-1.4-1.7-1.6-2-.2-.3 0-.5.1-.6.1-.1.3-.3.4-.5.1-.2.2-.3.2-.5.1-.2 0-.4 0-.5 0-.1-.7-1.6-.9-2.2-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.5.1-.8.4-.3.3-1 1-1 2.4 0 1.4 1 2.8 1.2 3 .1.2 2 3.1 4.9 4.3.7.3 1.2.5 1.6.6.7.2 1.3.2 1.8.1.5-.1 1.7-.7 1.9-1.4.2-.7.2-1.2.2-1.4 0-.1-.2-.2-.4-.3z"/><path d="M12 1C5.9 1 1 5.9 1 12c0 2 .5 3.9 1.5 5.6L1 23l5.5-1.5c1.6.9 3.5 1.4 5.5 1.4 6.1 0 11-4.9 11-11S18.1 1 12 1zm0 20c-1.7 0-3.3-.5-4.7-1.3l-.3-.2-3.5 1 1-3.4-.2-.4C3.5 15.3 3 13.7 3 12c0-5 4-9 9-9s9 4 9 9-4 9-9 9z"/></svg>
      Vamos conversar
    </a>
    <button class="nav-toggle" id="navToggle" aria-label="Abrir menu" aria-expanded="false" @click="toggleNav">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M4 6h16M4 12h16M4 18h16"/></svg>
    </button>
  </nav>
</template>

<script setup>
import { onMounted } from 'vue';

const toggleNav = () => {
  const navEl = document.getElementById('nav');
  const navToggle = document.getElementById('navToggle');
  const open = navEl.classList.toggle('is-open');
  if(navToggle) navToggle.setAttribute('aria-expanded', open);
};

onMounted(() => {
  const sections = document.querySelectorAll('section[id]');
  const navLinks = document.querySelectorAll('.nav-link');
  const setActive = () => {
    const y = window.scrollY + window.innerHeight * 0.35;
    let current = sections[0]?.id;
    sections.forEach(s => { if (s.offsetTop <= y) current = s.id; });
    navLinks.forEach(a => a.classList.toggle('active', a.getAttribute('href') === '#' + current));
  };
  window.addEventListener('scroll', setActive, { passive: true });
  setActive();

  const navEl = document.getElementById('nav');
  if(navEl) {
    navEl.querySelectorAll('.nav-link, .nav-cta').forEach(a => a.addEventListener('click', () => navEl.classList.remove('is-open')));
  }
});
</script>
