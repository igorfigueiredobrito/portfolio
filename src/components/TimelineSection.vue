<template>
    <section id="timeline" class="timeline-section" aria-labelledby="tl-h">
      <div class="container-narrow">
        <div class="section-meta reveal">
          <span class="num">§ 03</span>
          <span class="name">Carreira / Trajetória</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow">Carreira</span>
          <h2 id="tl-h" class="section-title">Uma trajetória contínua em <em>desenvolvedor de software</em></h2>
          <p class="section-sub">Da curiosidade aos 11 anos ao SaaS atendendo +200 fisioterapeutas. Cada parada foi uma evolução técnica e de produto.</p>
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
                  <h3 class="tl-company">Plusoft InPaaS<span class="sup">i</span></h3>
                  <div class="tl-role">Desenvolvedor Full Stack Sênior</div>
                </div>
                <span class="tl-date">Mar/2024 → hoje</span>
              </div>
              <p class="tl-summary">Desenvolvimento e customização da plataforma <strong>Hike</strong> — solução enterprise de <strong>BPM, CRM e Gestão Comercial</strong>. Responsável por integrações REST, automação de fluxos, novas funcionalidades e <em>otimização de processos</em> para grandes clientes.</p>
              <div class="tl-stack">
                <span class="tl-tag brand">Java</span>
                <span class="tl-tag brand">AngularJS</span>
                <span class="tl-tag">JavaScript</span>
                <span class="tl-tag">SQL Server</span>
                <span class="tl-tag">REST API</span>
                <span class="tl-tag">BPM</span>
              </div>
            </div>
          </article>

          <article class="tl-item">
            <span class="tl-dot" aria-hidden="true"></span>
            <div class="tl-card">
              <div class="tl-header">
                <div>
                  <div class="tl-meta-left" style="margin-bottom:10px;">
                    <span class="tl-index">2023 — 2024</span>
                  </div>
                  <h3 class="tl-company">Edusense</h3>
                  <div class="tl-role">Desenvolvedor Full Stack Pleno</div>
                </div>
                <span class="tl-date">Fev/2023 → Mar/2024</span>
              </div>
              <p class="tl-summary">Plataforma educacional com arquitetura híbrida — AngularJS legado migrando para <strong>Vue 3 + Tailwind</strong>. Modernização incremental, novas features e refatoração de telas críticas.</p>
              <div class="tl-stack">
                <span class="tl-tag brand">Vue 3</span>
                <span class="tl-tag">AngularJS</span>
                <span class="tl-tag">Tailwind CSS</span>
                <span class="tl-tag">Bootstrap 5</span>
                <span class="tl-tag">SQL Server</span>
              </div>
            </div>
          </article>
          
          <article class="tl-item">
            <span class="tl-dot" aria-hidden="true"></span>
            <div class="tl-card">
              <div class="tl-header">
                <div>
                  <div class="tl-meta-left" style="margin-bottom:10px;">
                    <span class="tl-index">2022 — 2023</span>
                  </div>
                  <h3 class="tl-company">bRHain</h3>
                  <div class="tl-role">Desenvolvedor Full Stack Pleno</div>
                </div>
                <span class="tl-date">Fev/2022 → Fev/2023</span>
              </div>
              <p class="tl-summary">Produto SaaS de RH e gestão de pessoas. Atuei na ponta full stack com foco em <strong>Vue 3 + AngularJS</strong>, dashboards analíticos e regras de negócio complexas em SQL Server.</p>
              <div class="tl-stack">
                <span class="tl-tag brand">Vue 3</span>
                <span class="tl-tag">AngularJS</span>
                <span class="tl-tag">Bootstrap 5</span>
                <span class="tl-tag">SQL Server</span>
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
