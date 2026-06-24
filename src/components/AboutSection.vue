<template>
    <section id="about" class="about" aria-labelledby="about-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num">§ 02</span>
          <span class="name">Sobre / About</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow">Quem está por trás</span>
          <h2 id="about-h" class="section-title">Estudante por dedicação, <em style="color: #16a34a;">desenvolvedor por vocação</em></h2>
          <p class="section-sub">Engenharia disciplinada, código limpo e foco em integrar software e hardware — não só linhas em produção.</p>
        </header>

        <div class="about-grid">
          <div class="about-bio reveal" data-d="1">
            <p class="lead">
              Sou estudante de Engenharia da Computação, movido pela curiosidade de entender como as coisas funcionam por baixo dos panos. Utilizando meu ambiente macOS, dedico-me a construir soluções que vão desde a interface do usuário até a comunicação direta com os servidores.
            </p>
            <p>
              Tenho forte atuação no desenvolvimento full-stack, criando aplicações móveis, sistemas de responsabilização e APIs de gestão. Minha stack técnica inclui o domínio de React Native, PHP, Java e Python (Django). Além da programação, construo e gerencio ecossistemas de infraestrutura de TI, elaborando dashboards detalhados no Grafana e orquestrando automações robustas via Zabbix e N8N.
            </p>
            <p>
              No mundo físico, aplico meus conhecimentos em projetos de hardware e IoT. Transformo teoria em prática desenvolvendo protótipos com microcontroladores ESP8266 e ESP32, desde maquetes de estacionamento com sensores ultrassônicos até sistemas de medição de empuxo para motores.
            </p>
            <p style="font-family:var(--font-serif);font-size:22px;font-style:italic;color:var(--ink);line-height:1.4;margin-top:32px;">
              Mais do que escrever código — construo infraestruturas que conectam o digital ao mundo real.
            </p>

            <div class="about-signature">
              <span class="sig">Igor</span>
              <div class="who">
                <strong>Igor Brito</strong>
                <span>Desenvolvedor Full-Stack & Estudante de Engenharia</span>
              </div>
            </div>
          </div>

          <aside class="reveal" data-d="2">
            <div class="about-card">
              <div class="about-card-photo">
                <img src="../assets/minha-foto.jpeg" alt="Igor Brito — desenvolvedor de software" width="420" height="525" loading="lazy" />
                <span class="tag" style="background-color: #dcfce7; color: #166534;"><span class="d" style="background-color: #166534;"></span>STATUS: Disponível p/ Projetos</span>
                <div class="stamp">
                  <span>TAG: IGOR BRITO / 2026</span>
                  <span>LOCAL: São Paulo, SP - BR</span>
                </div>
              </div>
              <div class="about-card-info">
                <div class="info-row"><span class="k">Empresa</span><span class="v">Plusoft InPaaS</span></div>
                <div class="info-row"><span class="k">Local</span><span class="v">São José dos Campos, SP · BR</span></div>
                <div class="info-row"><span class="k">Foco</span><span class="v">SaaS · Enterprise · Web</span></div>
                <div class="info-row"><span class="k">Stack</span><span class="v">Laravel · Vue · Java · AngularJS</span></div>
                <div class="info-row"><span class="k">Email</span><span class="v"><a href="mailto:contato@igorbrito.com">contato@igorbrito.com</a></span></div>
                <div class="info-row"><span class="k">Status</span><span class="v dotted">Aceitando projetos</span></div>
                <a href="https://api.whatsapp.com/send?phone=5511999999999" target="_blank" rel="noopener" class="about-card-cta">
                  <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor"><path d="M17.5 14.4c-.3-.1-1.7-.8-2-.9-.3-.1-.5-.1-.7.1-.2.3-.7.9-.9 1.1-.2.2-.3.2-.6.1-.3-.1-1.2-.4-2.3-1.4-.9-.8-1.4-1.7-1.6-2-.2-.3 0-.5.1-.6.1-.1.3-.3.4-.5.1-.2.2-.3.2-.5.1-.2 0-.4 0-.5 0-.1-.7-1.6-.9-2.2-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.5.1-.8.4-.3.3-1 1-1 2.4 0 1.4 1 2.8 1.2 3 .1.2 2 3.1 4.9 4.3.7.3 1.2.5 1.6.6.7.2 1.3.2 1.8.1.5-.1 1.7-.7 1.9-1.4.2-.7.2-1.2.2-1.4 0-.1-.2-.2-.4-.3z"/><path d="M12 1C5.9 1 1 5.9 1 12c0 2 .5 3.9 1.5 5.6L1 23l5.5-1.5c1.6.9 3.5 1.4 5.5 1.4 6.1 0 11-4.9 11-11S18.1 1 12 1zm0 20c-1.7 0-3.3-.5-4.7-1.3l-.3-.2-3.5 1 1-3.4-.2-.4C3.5 15.3 3 13.7 3 12c0-5 4-9 9-9s9 4 9 9-4 9-9 9z"/></svg>
                  Enviar mensagem
                </a>
              </div>
            </div>
          </aside>
        </div>

        <div class="metrics reveal" data-d="3">
          <div class="metric"><div class="num" data-count="8"><span>8</span><em>+</em></div><div class="lbl">Anos de experiência</div></div>
          <div class="metric"><div class="num" data-count="9"><span>9</span></div><div class="lbl">Empresas atendidas</div></div>
          <div class="metric"><div class="num" data-count="10"><span>10</span><em>+</em></div><div class="lbl">Projetos entregues</div></div>
          <div class="metric"><div class="num" data-count="200"><span>200</span><em>+</em></div><div class="lbl">Usuários no Fisioly</div></div>
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
  document.querySelectorAll('#about .reveal').forEach(el => io.observe(el));

  const metricEls = document.querySelectorAll('.metric .num[data-count]');
  const counterIO = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (!entry.isIntersecting) return;
      const el = entry.target;
      const target = parseInt(el.getAttribute('data-count'), 10);
      const span = el.querySelector('span');
      if (!span) return;
      const dur = 1400;
      const start = performance.now();
      const startVal = 0;
      function step(now) {
        const t = Math.min(1, (now - start)/dur);
        const eased = 1 - Math.pow(1 - t, 3);
        const val = Math.round(startVal + (target - startVal) * eased);
        span.textContent = val.toLocaleString('pt-BR');
        if (t < 1) requestAnimationFrame(step);
      }
      requestAnimationFrame(step);
      counterIO.unobserve(el);
    });
  }, { threshold: 0.4 });
  metricEls.forEach(el => counterIO.observe(el));
});
</script>
