<template>
    <section id="home" class="hero" aria-labelledby="hero-name">
      <div class="hero-bg" aria-hidden="true">
        <span class="orb o1"></span>
        <span class="orb o2"></span>
        <span class="orb o3"></span>
      </div>
      <div class="hero-vignette" aria-hidden="true"></div>
      <div class="hero-grid" aria-hidden="true"></div>
      <div class="hero-spotlight" aria-hidden="true"></div>

      <div class="container">
        <div class="hero-meta">
          <div class="left">
            <span class="eyebrow">Portfolio · MMXXVI</span>
            <span class="badge">
              <span class="dot-wrap">Disponível</span>
              Aceitando projetos para 2026
            </span>
          </div>
          <div class="right">
            <span class="loc">São José dos Campos · SP — Brasil</span>
            <span class="time"><span class="pulse2"></span><span id="liveClock">{{ time }}</span> BRT</span>
          </div>
        </div>

        <div class="hero-stage">
          <div class="hero-text">
            <div class="hero-tag-row">
              <span class="num">N° 01</span>
              <span class="sep"></span>
              <span>Desenvolvedor · Founder · Builder</span>
            </div>

            <h1 id="hero-name" class="hero-name">
              <span class="row"><span class="word">Igor</span></span>
              <span class="row"><span class="word prado">Brito</span></span>
            </h1>

            <div class="hero-role">
              <span class="role-pill">Desenvolvedor Full Stack <em>Sênior</em></span>
              <span class="mono" style="font-size:12px;color:var(--muted);">— hoje na Plusoft InPaaS · founder do Fisioly</span>
            </div>

            <p class="hero-bio">
              Construo <strong>sistemas enterprise</strong>, APIs escaláveis e produtos SaaS que sustentam negócios reais. <em>8+ anos</em> entregando software com Laravel, Vue, Angular, Java e Flutter — do MVP de fim de semana à plataforma BPM que serve grandes operações.
            </p>

            <div class="hero-actions">
              <a href="#contact" class="btn btn-lg btn-primary" data-magnetic>
                <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M17.5 14.4c-.3-.1-1.7-.8-2-.9-.3-.1-.5-.1-.7.1-.2.3-.7.9-.9 1.1-.2.2-.3.2-.6.1-.3-.1-1.2-.4-2.3-1.4-.9-.8-1.4-1.7-1.6-2-.2-.3 0-.5.1-.6.1-.1.3-.3.4-.5.1-.2.2-.3.2-.5.1-.2 0-.4 0-.5 0-.1-.7-1.6-.9-2.2-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.5.1-.8.4-.3.3-1 1-1 2.4 0 1.4 1 2.8 1.2 3 .1.2 2 3.1 4.9 4.3.7.3 1.2.5 1.6.6.7.2 1.3.2 1.8.1.5-.1 1.7-.7 1.9-1.4.2-.7.2-1.2.2-1.4 0-.1-.2-.2-.4-.3z"/><path d="M12 1C5.9 1 1 5.9 1 12c0 2 .5 3.9 1.5 5.6L1 23l5.5-1.5c1.6.9 3.5 1.4 5.5 1.4 6.1 0 11-4.9 11-11S18.1 1 12 1zm0 20c-1.7 0-3.3-.5-4.7-1.3l-.3-.2-3.5 1 1-3.4-.2-.4C3.5 15.3 3 13.7 3 12c0-5 4-9 9-9s9 4 9 9-4 9-9 9z"/></svg>
                Fale comigo
              </a>
              <a href="#timeline" class="btn btn-lg btn-glass">
                Ver trajetória
                <span class="arrow"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" aria-hidden="true"><path d="M5 12h14M13 6l6 6-6 6"/></svg></span>
              </a>
            </div>
          </div>

          <div class="hero-portrait" data-tilt>
            <div class="hero-portrait-frame">
              <!-- Placeholder image since local is not available -->
              <img src="../assets/minha-foto.jpeg" alt="Retrato" width="420" height="560" loading="eager" />
              <div class="frame-corner tl" aria-hidden="true"></div>
              <div class="frame-corner tr" aria-hidden="true"></div>
              <div class="frame-corner bl" aria-hidden="true"></div>
              <div class="frame-corner br" aria-hidden="true"></div>
              <div class="frame-label">
                <span class="l">IB · 01</span>
                <span class="r">f/2.8 · TBT</span>
              </div>
            </div>
            <span class="float-tag t1"><span class="d"></span>Sênior · 8+ anos</span>
            <span class="float-tag t2"><span class="d"></span>Founder · Fisioly</span>
            <span class="float-tag t3"><span class="d"></span>Plusoft · InPaaS</span>
          </div>
        </div>

        <div class="hero-strip">
          <span class="label">Stack</span>
          <div class="stack-marquee">
            <div class="stack-marquee-inner">
              <span class="stack-item"><span class="marker"></span>Laravel</span>
              <span class="stack-item"><span class="marker"></span>PHP 8</span>
              <span class="stack-item"><span class="marker"></span>Java</span>
              <span class="stack-item"><span class="marker"></span>Vue 3</span>
              <span class="stack-item"><span class="marker"></span>Angular</span>
              <span class="stack-item"><span class="marker"></span>Flutter</span>
              <span class="stack-item"><span class="marker"></span>Ionic</span>
              <span class="stack-item"><span class="marker"></span>Node.js</span>
              <span class="stack-item"><span class="marker"></span>TypeScript</span>
              <span class="stack-item"><span class="marker"></span>AWS</span>
              <span class="stack-item"><span class="marker"></span>Docker</span>
              <!-- Duplicate for seamless loop -->
              <span class="stack-item"><span class="marker"></span>Laravel</span>
              <span class="stack-item"><span class="marker"></span>PHP 8</span>
              <span class="stack-item"><span class="marker"></span>Java</span>
              <span class="stack-item"><span class="marker"></span>Vue 3</span>
              <span class="stack-item"><span class="marker"></span>Angular</span>
              <span class="stack-item"><span class="marker"></span>Flutter</span>
              <span class="stack-item"><span class="marker"></span>Ionic</span>
              <span class="stack-item"><span class="marker"></span>Node.js</span>
              <span class="stack-item"><span class="marker"></span>TypeScript</span>
              <span class="stack-item"><span class="marker"></span>AWS</span>
              <span class="stack-item"><span class="marker"></span>Docker</span>
            </div>
          </div>
          <span class="hero-scroll-hint">Role <span class="arrow-line"></span></span>
        </div>
      </div>
    </section>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue';

const time = ref('--:--');
let interval;

onMounted(() => {
  const tick = () => {
    const now = new Date();
    const fmt = new Intl.DateTimeFormat('pt-BR', { hour: '2-digit', minute: '2-digit', timeZone: 'America/Sao_Paulo', hour12: false });
    time.value = fmt.format(now);
  };
  tick();
  interval = setInterval(tick, 30000);

  const hero = document.querySelector('.hero');
  if (hero && window.matchMedia('(hover: hover)').matches) {
    let raf = null;
    hero.addEventListener('mousemove', (e) => {
      if (raf) return;
      raf = requestAnimationFrame(() => {
        const r = hero.getBoundingClientRect();
        const x = ((e.clientX - r.left) / r.width) * 100;
        const y = ((e.clientY - r.top) / r.height) * 100;
        hero.style.setProperty('--mx', x + '%');
        hero.style.setProperty('--my', y + '%');
        raf = null;
      });
    }, { passive: true });
  }

  const tiltEl = document.querySelector('[data-tilt]');
  if (tiltEl && window.matchMedia('(hover: hover)').matches) {
    const frame = tiltEl.querySelector('.hero-portrait-frame');
    tiltEl.addEventListener('mousemove', (e) => {
      const r = tiltEl.getBoundingClientRect();
      const cx = r.left + r.width/2;
      const cy = r.top + r.height/2;
      const dx = (e.clientX - cx) / (r.width/2);
      const dy = (e.clientY - cy) / (r.height/2);
      if(frame) frame.style.transform = `perspective(1000px) rotateY(${dx*6}deg) rotateX(${-dy*5}deg) translateZ(0)`;
    });
    tiltEl.addEventListener('mouseleave', () => {
      if(frame) frame.style.transform = '';
    });
  }

  document.querySelectorAll('[data-magnetic]').forEach(btn => {
    if (!window.matchMedia('(hover: hover)').matches) return;
    btn.addEventListener('mousemove', (e) => {
      const r = btn.getBoundingClientRect();
      const cx = r.left + r.width/2;
      const cy = r.top + r.height/2;
      const dx = (e.clientX - cx) * .22;
      const dy = (e.clientY - cy) * .22;
      btn.style.transform = `translate(${dx}px, ${dy}px)`;
    });
    btn.addEventListener('mouseleave', () => {
      btn.style.transform = '';
    });
  });
});

onUnmounted(() => {
  clearInterval(interval);
});
</script>
