<template>
    <section id="timeline" class="timeline-section" aria-labelledby="tl-h">
      <div class="container-narrow">
        <div class="section-meta reveal">
          <span class="num">§ 03</span>
          <span class="name">Carreira / Trajetória</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow">Carreira</span>
          <h2 id="tl-h" class="section-title">Uma trajetória de evolução em <em>engenharia e infraestrutura</em></h2>
          <p class="section-sub">Da base em suporte técnico e redes ao desenvolvimento full-stack de soluções corporativas. Cada etapa construiu minha visão sistêmica sobre tecnologia.</p>
        </header>

        <div class="timeline" id="timelineInner">
          <div class="timeline-progress" id="tlProgress" aria-hidden="true"></div>

          <article class="tl-item">
            <span class="tl-dot" aria-hidden="true"></span>
            <div class="tl-card">
              <div class="tl-header">
                <div>
                  <div class="tl-meta-left" style="margin-bottom:10px;">
                    <span class="tl-index">2024 — hoje</span>
                    <span class="tl-current">● Atualmente</span>
                  </div>
                  <h3 class="tl-company">Visiona Tecnologia Espacial<span class="sup">i</span></h3>
                  <div class="tl-role">Estagiário em T.I.</div>
                </div>
                <span class="tl-date">Jul/2024 → hoje</span>
              </div>
              <p class="tl-summary">Desenvolvimento full-stack e automação de plataformas internas utilizando Python (Back-end) e Vue.js/JavaScript (Front-end). Atuação na criação de APIs REST, manipulação de dados (JSON) e estruturação de dashboards analíticos no Grafana para monitoramento em tempo real de infraestrutura.</p>
              <div class="tl-stack">
                <span class="tl-tag brand">Python</span>
                <span class="tl-tag brand">Vue.js</span>
                <span class="tl-tag">Grafana</span>
                <span class="tl-tag">API REST</span>
                <span class="tl-tag">Zscaler</span>
                <span class="tl-tag">Linux</span>
              </div>
            </div>
          </article>

          <article class="tl-item">
            <span class="tl-dot" aria-hidden="true"></span>
            <div class="tl-card">
              <div class="tl-header">
                <div>
                  <div class="tl-meta-left" style="margin-bottom:10px;">
                    <span class="tl-index">2022 — 2024</span>
                  </div>
                  <h3 class="tl-company">Info Uai Ltda.</h3>
                  <div class="tl-role">Técnico em Informática</div>
                </div>
                <span class="tl-date">Mar/2022 → Jul/2024</span>
              </div>
              <p class="tl-summary">Implantação e administração de Servidores Windows e infraestrutura avançada de redes (Firewalls, Switches, Access Points). Gestão de soluções corporativas de segurança e backup utilizando Kaspersky e Veeam, além da orquestração de comunicação em nuvem e gerenciamento de ativos.</p>
              <div class="tl-stack">
                <span class="tl-tag brand">Windows Server</span>
                <span class="tl-tag">Redes & Firewall</span>
                <span class="tl-tag">Veeam</span>
                <span class="tl-tag">Kaspersky</span>
                <span class="tl-tag">Hardware</span>
              </div>
            </div>
          </article>
          
          <article class="tl-item">
            <span class="tl-dot" aria-hidden="true"></span>
            <div class="tl-card">
              <div class="tl-header">
                <div>
                  <div class="tl-meta-left" style="margin-bottom:10px;">
                    <span class="tl-index">2021 — 2021</span>
                  </div>
                  <h3 class="tl-company">Prefeitura Municipal de S. J. Campos</h3>
                  <div class="tl-role">Estagiário em Informática</div>
                </div>
                <span class="tl-date">Jun/2021 → Nov/2021</span>
              </div>
              <p class="tl-summary">Atuação no suporte corporativo com foco em manutenção preventiva e corretiva de hardware. Auxílio direto na instalação de softwares, reparos de estações de trabalho e suporte resolutivo aos usuários finais na utilização dos sistemas internos do setor público.</p>
              <div class="tl-stack">
                <span class="tl-tag brand">Suporte Técnico</span>
                <span class="tl-tag">Manutenção</span>
                <span class="tl-tag">Help Desk</span>
                <span class="tl-tag">Troubleshooting</span>
              </div>
            </div>
          </article>

        </div>
      </div>
    </section>
</template>

<script setup>
import { onMounted } from 'vue';

onMounted(() => {
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) { e.target.classList.add('in'); io.unobserve(e.target); }
    });
  }, { rootMargin: '0px 0px -40px 0px', threshold: 0.06 });
  document.querySelectorAll('#timeline .reveal').forEach(el => io.observe(el));

  const tlItems = document.querySelectorAll('.tl-item');
  const tlIO = new IntersectionObserver((entries) => {
    entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('in'); tlIO.unobserve(e.target); } });
  }, { rootMargin: '0px 0px -80px 0px', threshold: 0.12 });
  tlItems.forEach(i => tlIO.observe(i));

  const tl = document.getElementById('timelineInner');
  const tlProgress = document.getElementById('tlProgress');
  if (tl && tlProgress) {
    let raf2 = null;
    const onScroll = () => {
      if (raf2) return;
      raf2 = requestAnimationFrame(() => {
        const r = tl.getBoundingClientRect();
        const total = r.height;
        const vh = window.innerHeight;
        const start = r.top;
        let p = 0;
        if (start < vh * 0.5) {
          p = Math.min(1, Math.max(0, (vh * 0.5 - start) / (total - vh * 0.4)));
        }
        tlProgress.style.height = (p * 100) + '%';
        raf2 = null;
      });
    };
    window.addEventListener('scroll', onScroll, { passive: true });
    onScroll();
  }
});
</script>
