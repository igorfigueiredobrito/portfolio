<template>
  <HeaderNav />
  <main>
    <HeroSection />
    <AboutSection />
    <TimelineSection />

    <!-- Additional Sections directly in App.vue for brevity -->
    <!-- STACK -->
    <section id="stack" class="stack-section" aria-labelledby="stack-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num">N° 04</span>
          <span class="name">Stack / Toolbox</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow">Ferramentas</span>
          <h2 id="stack-h" class="section-title">A oficina, <em>arrumada</em></h2>
          <p class="section-sub">Tecnologias que uso diariamente em produção — escolhidas pelo que entregam, não pela última moda.</p>
        </header>

        <div class="stack-grid reveal" data-d="1">
          <div class="stack-col">
            <div class="stack-col-head">Back-end & Dados</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">Py</span>Python (Django, FastAPI, Flask)</div>
              <div class="stack-pill"><span class="ico">J/P</span>Java & PHP</div>
              <div class="stack-pill"><span class="ico">Db</span>MySQL & MongoDB</div>
              <div class="stack-pill"><span class="ico">Api</span>APIs REST & JSON</div>
            </div>
          </div>
          <div class="stack-col">
            <div class="stack-col-head">Front-end</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">Js</span>JavaScript</div>
              <div class="stack-pill"><span class="ico">V</span>Vue.js</div>
              <div class="stack-pill"><span class="ico">N</span>Node.js</div>
              <div class="stack-pill"><span class="ico">Ui</span>Integração de Interfaces</div>
            </div>
          </div>
          <div class="stack-col">
            <div class="stack-col-head">Infraestrutura & Redes</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">Os</span>Linux & Windows Server</div>
              <div class="stack-pill"><span class="ico">D/G</span>Docker & Git</div>
              <div class="stack-pill"><span class="ico">Px</span>Proxmox / Virtualização</div>
              <div class="stack-pill"><span class="ico">Sec</span>Fortinet & Zscaler (Segurança)</div>
            </div>
          </div>
          <div class="stack-col">
            <div class="stack-col-head">Automação, IoT & IA</div>
            <div class="stack-list">
              <div class="stack-pill"><span class="ico">G/Z</span>Grafana & Zabbix</div>
              <div class="stack-pill"><span class="ico">n8n</span>n8n (Webhooks/Automação)</div>
              <div class="stack-pill"><span class="ico">IoT</span>ESP32 / ESP8266</div>
              <div class="stack-pill"><span class="ico">IA</span>Modelos LLM (LLaMA / Gemini)</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services" class="services" aria-labelledby="svc-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num">N° 05</span>
          <span class="name">Serviços / What I do</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow">— O QUE EU FAÇO</span>
          <h2 id="svc-h" class="section-title">Engenharia que <em>vai além do código</em></h2>
          <p class="section-sub">Especialidades técnicas focadas na construção de ecossistemas completos, unindo desenvolvimento de software, automação e infraestrutura para negócios reais.</p>
        </header>

        <div class="services-grid reveal" data-d="1">
          <article class="svc-card">
            <div class="svc-num">01 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
            </div>
            <h3 class="svc-title">Desenvolvimento <em>Full Stack</em></h3>
            <p class="svc-desc">Sistemas web completos com arquitetura limpa e escalável. Construo back-ends robustos e seguros utilizando Python (Django/FastAPI), Java ou PHP, e interfaces modernas e dinâmicas no front-end com JavaScript e Vue.js.</p>
          </article>
          <article class="svc-card">
            <div class="svc-num">02 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="3" width="20" height="14" rx="2" ry="2"/><line x1="8" y1="21" x2="16" y2="21"/><line x1="12" y1="17" x2="12" y2="21"/></svg>
            </div>
            <h3 class="svc-title">Websites &amp; <em>Plataformas SaaS</em></h3>
            <p class="svc-desc">Criação de produtos digitais de ponta a ponta. Desenvolvo desde landing pages institucionais otimizadas até sistemas SaaS complexos com controle financeiro, painéis gerenciais (dashboards) e modelagem de banco de dados SQL/NoSQL.</p>
          </article>
          <article class="svc-card">
            <div class="svc-num">03 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg>
            </div>
            <h3 class="svc-title">APIs &amp; <em>Integrações</em></h3>
            <p class="svc-desc">Desenvolvimento e integração de APIs RESTful seguras. Especialista em conectar sistemas independentes utilizando webhooks, n8n, serviços de terceiros e em estruturar a comunicação de dados em formatos JSON.</p>
          </article>
          <article class="svc-card">
            <div class="svc-num">04 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"/><line x1="12" y1="20" x2="12" y2="4"/><line x1="6" y1="20" x2="6" y2="14"/></svg>
            </div>
            <h3 class="svc-title">Monitoramento &amp; <em>Dados</em></h3>
            <p class="svc-desc">Transformação de dados brutos em inteligência visual. Criação de dashboards centralizados no Grafana e Zabbix para monitoramento em tempo real de redes, servidores e métricas de negócio.</p>
          </article>
          <article class="svc-card">
            <div class="svc-num">05 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="2" width="20" height="8" rx="2" ry="2"/><rect x="2" y="14" width="20" height="8" rx="2" ry="2"/><line x1="6" y1="6" x2="6.01" y2="6"/><line x1="6" y1="18" x2="6.01" y2="18"/></svg>
            </div>
            <h3 class="svc-title">Infraestrutura &amp; <em>Redes</em></h3>
            <p class="svc-desc">Administração e sustentação de ambientes corporativos. Atuação com servidores Linux/Windows, virtualização (Proxmox, VirtualBox), segurança em nuvem e conteinerização com Docker.</p>
          </article>
          <article class="svc-card">
            <div class="svc-num">06 / 06</div>
            <div class="svc-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="4" width="16" height="16" rx="2" ry="2"/><rect x="9" y="9" width="6" height="6"/><line x1="9" y1="1" x2="9" y2="4"/><line x1="15" y1="1" x2="15" y2="4"/><line x1="9" y1="20" x2="9" y2="23"/><line x1="15" y1="20" x2="15" y2="23"/><line x1="20" y1="9" x2="23" y2="9"/><line x1="20" y1="14" x2="23" y2="14"/><line x1="1" y1="9" x2="4" y2="9"/><line x1="1" y1="14" x2="4" y2="14"/></svg>
            </div>
            <h3 class="svc-title">Automação IoT &amp; <em>IA</em></h3>
            <p class="svc-desc">Integração de hardware e inteligência ao software. Projetos de automação com microcontroladores (ESP32/ESP8266), sensores e implantação de modelos de Inteligência Artificial locais (LLMs) para consumo via API.</p>
          </article>
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="contact" aria-labelledby="contact-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num">N° 06</span>
          <span class="name">Contato / Let's talk</span>
        </div>
        <div class="contact-card reveal">
          <div class="contact-intro">
            <div class="marker">Disponível para 2026</div>
            <h3 id="contact-h">Tem um projeto <em>em mente</em>?</h3>
            <p>Estou disponível para projetos freelance, consultorias e parcerias. Respondo geralmente em poucas horas. A forma mais rápida é pelo WhatsApp.</p>
            <div style="margin-top:32px;display:flex;gap:10px;flex-wrap:wrap;">
              <a href="https://api.whatsapp.com/send?phone=5512982112088" target="_blank" rel="noopener" class="btn btn-lg btn-whatsapp" data-magnetic>
                WhatsApp direto
              </a>
            </div>
          </div>
          <div class="contact-channels">
            <!-- WhatsApp -->
            <a href="https://api.whatsapp.com/send?phone=5512982112088" target="_blank" rel="noopener" class="channel">
              <div class="channel-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 11.5a8.38 8.38 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.38 8.38 0 0 1-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.38 8.38 0 0 1 3.8-.9h.5a8.48 8.48 0 0 1 8 8v.5z"></path></svg>
              </div>
              <div class="channel-info">
                <div class="k">WHATSAPP</div>
                <div class="v">+55 (12) 98211-2088</div>
              </div>
              <div class="channel-arrow">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
              </div>
            </a>
            <!-- Email -->
            <a href="mailto:igorfigueiredobrito@gmail.com" class="channel">
              <div class="channel-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
              </div>
              <div class="channel-info">
                <div class="k">EMAIL</div>
                <div class="v">igorfigueiredobrito@gmail.com</div>
              </div>
              <div class="channel-arrow">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
              </div>
            </a>
            <!-- LinkedIn -->
            <a href="https://www.linkedin.com/in/igor-f-brito/" target="_blank" rel="noopener" class="channel">
              <div class="channel-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle></svg>
              </div>
              <div class="channel-info">
                <div class="k">LINKEDIN</div>
                <div class="v">linkedin.com/in/igor-f-brito</div>
              </div>
              <div class="channel-arrow">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
              </div>
            </a>
            <!-- GitHub -->
            <a href="https://github.com/igorfigueiredobrito" target="_blank" rel="noopener" class="channel">
              <div class="channel-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>
              </div>
              <div class="channel-info">
                <div class="k">GITHUB</div>
                <div class="v">github.com/igorfigueiredobrito</div>
              </div>
              <div class="channel-arrow">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
              </div>
            </a>
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
        <div class="footer-social">
          <a href="https://www.linkedin.com/in/igor-f-brito/" target="_blank" rel="noopener" aria-label="LinkedIn">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle></svg>
          </a>
          <a href="https://github.com/igorfigueiredobrito" target="_blank" rel="noopener" aria-label="GitHub">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>
          </a>
          <a href="https://instagram.com/" target="_blank" rel="noopener" aria-label="Instagram">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>
          </a>
          <a href="/cv.pdf" download="Currículo - Igor Brito.pdf" aria-label="Download CV">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import HeaderNav from './components/HeaderNav.vue';
import HeroSection from './components/HeroSection.vue';
import AboutSection from './components/AboutSection.vue';
import TimelineSection from './components/TimelineSection.vue';

import { onMounted } from 'vue';

onMounted(() => {
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) { e.target.classList.add('in'); io.unobserve(e.target); }
    });
  }, { rootMargin: '0px 0px -40px 0px', threshold: 0.06 });
  document.querySelectorAll('main > section:not(#home):not(#about):not(#timeline) .reveal, .footer .reveal').forEach(el => io.observe(el));
});
</script>
