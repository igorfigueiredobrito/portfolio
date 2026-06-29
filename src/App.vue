<template>
  <HeaderNav />
  <main>
    <HeroSection />
    <AboutSection />
    <TimelineSection />
    <FisiolySection />

    <!-- Additional Sections directly in App.vue for brevity -->
    <!-- STACK -->
    <section id="stack" class="stack-section" aria-labelledby="stack-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num">§ 05</span>
          <span class="name">Stack / Toolbox</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow">Ferramentas</span>
          <h2 id="stack-h" class="section-title">A oficina, <em>arrumada</em></h2>
          <p class="section-sub">Tecnologias que uso diariamente em produção — escolhidas pelo que entregam, não pela última moda.</p>
        </header>

        <div class="stack-grid reveal" data-d="1">
          <div class="stack-col">
            <div class="stack-col-head">Back-end & APIs</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">Py</span>Python (Django, FastAPI)</div>
              <div class="stack-pill"><span class="ico">J</span>Java</div>
              <div class="stack-pill"><span class="ico">P</span>PHP</div>
            </div>
          </div>
          <div class="stack-col">
            <div class="stack-col-head">Front-end</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">Js</span>JavaScript (Vue.js, Node.js)</div>
            </div>
          </div>
          <div class="stack-col">
            <div class="stack-col-head">Infraestrutura & DevOps</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">D</span>Docker</div>
              <div class="stack-pill"><span class="ico">G</span>Git</div>
              <div class="stack-pill"><span class="ico">L</span>Linux</div>
              <div class="stack-pill"><span class="ico">Px</span>Proxmox</div>
              <div class="stack-pill"><span class="ico">C</span>AWS/GCP</div>
            </div>
          </div>
          <div class="stack-col">
            <div class="stack-col-head">Monitoramento & IoT</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">Gf</span>Grafana</div>
              <div class="stack-pill"><span class="ico">Z</span>Zabbix</div>
              <div class="stack-pill"><span class="ico">N</span>n8n</div>
              <div class="stack-pill"><span class="ico">E</span>ESP32/ESP8266</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services" class="services" aria-labelledby="svc-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num">§ 06</span>
          <span class="name">Serviços / What I do</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow">O que eu faço</span>
          <h2 id="svc-h" class="section-title">Engenharia que <em>vai além do código</em></h2>
          <p class="section-sub">Especialidades técnicas afiadas em 8+ anos entregando sistemas que sustentam negócios reais.</p>
        </header>

        <div class="services-grid reveal" data-d="1">
          <article class="svc-card">
            <div class="svc-num">01 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
            </div>
            <h3 class="svc-title">Desenvolvimento <em>Full Stack</em></h3>
            <p class="svc-desc">Sistemas web completos com arquitetura limpa, escalável e segura — back-end robusto em <strong>Laravel/PHP</strong> ou <strong>Java</strong> e front-end moderno em <strong>Vue.js</strong> ou <strong>Angular</strong>.</p>
          </article>
          <article class="svc-card">
            <div class="svc-num">02 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="5" y="2" width="14" height="20" rx="2"/><line x1="12" y1="18" x2="12.01" y2="18"/></svg>
            </div>
            <h3 class="svc-title">Aplicativos <em>Mobile</em></h3>
            <p class="svc-desc">Apps cross-platform performáticos com <strong>Flutter</strong> e <strong>Ionic</strong>, integrados a APIs REST e prontos para Android e iOS.</p>
          </article>
          <article class="svc-card">
            <div class="svc-num">03 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/><path d="M9 12l2 2 4-4"/></svg>
            </div>
            <h3 class="svc-title">APIs &amp; <em>Integrações</em></h3>
            <p class="svc-desc">Criação e integração de <strong>APIs RESTful</strong> robustas, webhooks, integrações com sistemas legados e serviços de terceiros — com documentação e testes.</p>
          </article>
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="contact" aria-labelledby="contact-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num">§ 08</span>
          <span class="name">Contato / Let's talk</span>
        </div>
        <div class="contact-card reveal">
          <div class="contact-intro">
            <div class="marker">Disponível para 2026</div>
            <h3 id="contact-h">Tem um projeto <em>em mente</em>?</h3>
            <p>Estou disponível para projetos freelance, consultorias e parcerias. Respondo geralmente em poucas horas. A forma mais rápida é pelo WhatsApp.</p>
            <div style="margin-top:32px;display:flex;gap:10px;flex-wrap:wrap;">
              <a href="https://api.whatsapp.com/send?phone=5511999999999" target="_blank" rel="noopener" class="btn btn-lg btn-whatsapp" data-magnetic>
                WhatsApp direto
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
  
  <footer class="footer" role="contentinfo">
    <div class="container">
      <div class="footer-mega reveal">Let's <em>build</em></div>
      <div class="footer-inner">
        <div class="footer-brand">
          <div class="mark"><img src="./assets/minha-foto.jpeg" alt="" width="44" height="44" /></div>
          <div class="info">
            <strong>Igor Brito</strong>
            <span>Desenvolvedor Full Stack · BR</span>
          </div>
        </div>
        <p class="footer-copy">© 2026 · Construído à mão · Movido a café</p>
      </div>
    </div>
  </footer>
</template>

<script setup>
import HeaderNav from './components/HeaderNav.vue';
import HeroSection from './components/HeroSection.vue';
import AboutSection from './components/AboutSection.vue';
import TimelineSection from './components/TimelineSection.vue';
import FisiolySection from './components/FisiolySection.vue';

import { onMounted } from 'vue';

onMounted(() => {
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) { e.target.classList.add('in'); io.unobserve(e.target); }
    });
  }, { rootMargin: '0px 0px -40px 0px', threshold: 0.06 });
  document.querySelectorAll('main > section:not(#home):not(#about):not(#timeline):not(#fisioly) .reveal, .footer .reveal').forEach(el => io.observe(el));
});
</script>
