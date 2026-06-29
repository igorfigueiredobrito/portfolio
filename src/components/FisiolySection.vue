<template>
    <section id="fisioly" class="fisioly" aria-labelledby="fisioly-h">
      <div class="container">
        <div class="section-meta reveal">
          <span class="num" style="color:#b282ff;">N° 04</span>
          <span class="name">Projeto SaaS principal</span>
        </div>
        <header class="section-header reveal">
          <span class="eyebrow fisioly-eyebrow">Featured Product</span>
          <h2 id="fisioly-h" class="section-title">Do código à <em>empresa de produto</em></h2>
          <p class="section-sub">Idealizei, projetei e construí o <strong style="color:var(--ink)">Fisioly</strong> — um SaaS B2B completo para fisioterapeutas e clínicas. Hoje atende mais de 200 profissionais ativos no Brasil.</p>
        </header>

        <div class="fisioly-card reveal" data-d="1">
          <div class="fisioly-grid">
            <div>
              <div class="fisioly-brand">
                <span class="fisioly-wordmark">Fisioly<span class="dot" aria-hidden="true"></span></span>
                <span class="fisioly-tag">SaaS · 2022</span>
              </div>

              <h3 class="fisioly-title">Sistema para fisioterapia que <em>transforma a clínica</em> em uma máquina de atendimentos.</h3>
              <p class="fisioly-desc">
                Agenda inteligente com lembretes por WhatsApp, prontuário eletrônico, evolução clínica e financeiro automático — tudo em uma plataforma rápida, segura e em conformidade com a LGPD. <strong>Reduz faltas em 35%</strong> e devolve mais de 15h por mês ao fisioterapeuta.
              </p>

              <div class="fisioly-stats">
                <div class="fisioly-stat"><div class="v"><em>+</em>200</div><div class="l">Profissionais ativos</div></div>
                <div class="fisioly-stat"><div class="v">35<em>%</em></div><div class="l">Menos faltas</div></div>
                <div class="fisioly-stat"><div class="v">4.9<em>★</em></div><div class="l">Avaliação média</div></div>
              </div>

              <a href="https://fisioly.com.br/" target="_blank" rel="noopener" class="fisioly-cta" title="Sistema para fisioterapia Fisioly" data-magnetic>
                Conhecer o sistema para fisioterapia
                <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" aria-hidden="true"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
              </a>

              <p class="fisioly-seo">
                Saiba mais sobre o <a href="https://fisioly.com.br/prontuario-eletronico-fisioterapia" target="_blank" rel="noopener">prontuário eletrônico de fisioterapia</a>.
              </p>
            </div>

            <div class="fisioly-dash" aria-hidden="true">
              <div class="fisioly-dash-inner">
                <div class="fd-chrome">
                  <i class="r"></i><i class="y"></i><i class="g"></i>
                  <span class="u">fisioly.com.br / dashboard</span>
                </div>
                <div class="fd-body">
                  <div class="fd-row1">
                    <div class="fd-stat"><div class="l">Sessões</div><div class="v">142</div><div class="d">↑ 18%</div></div>
                    <div class="fd-stat"><div class="l">Faturamento</div><div class="v">R$ 28k</div><div class="d">↑ 38%</div></div>
                    <div class="fd-stat"><div class="l">Pacientes</div><div class="v">186</div><div class="d">↑ 12</div></div>
                  </div>
                  <div class="fd-row2">
                    <div class="fd-chart">
                      <div class="fd-chart-head"><strong>Atendimentos</strong><span>Últimos 30 dias</span></div>
                      <svg viewBox="0 0 320 80" preserveAspectRatio="none">
                        <defs>
                          <linearGradient id="fdA" x1="0" y1="0" x2="0" y2="1">
                            <stop offset="0" stop-color="#8F3EFF" stop-opacity=".5"/>
                            <stop offset="1" stop-color="#8F3EFF" stop-opacity="0"/>
                          </linearGradient>
                          <linearGradient id="fdL" x1="0" x2="1" y1="0" y2="0">
                            <stop offset="0" stop-color="#8F3EFF"/>
                            <stop offset=".5" stop-color="#5670FF"/>
                            <stop offset="1" stop-color="#20E0C4"/>
                          </linearGradient>
                        </defs>
                        <path d="M0 60 L32 52 L64 56 L96 42 L128 48 L160 30 L192 38 L224 22 L256 26 L288 12 L320 16 L320 80 L0 80 Z" fill="url(#fdA)"/>
                        <path class="fd-line" d="M0 60 L32 52 L64 56 L96 42 L128 48 L160 30 L192 38 L224 22 L256 26 L288 12 L320 16" fill="none" stroke="url(#fdL)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                      </svg>
                    </div>
                    <div class="fd-list">
                      <div class="fd-list-h">Próximas sessões</div>
                      <div class="fd-list-row"><span class="t">09:00</span><span class="n">Mariana S.</span><span class="d"></span></div>
                      <div class="fd-list-row next"><span class="t">10:30</span><span class="n">Carlos M.</span><span class="d"></span></div>
                      <div class="fd-list-row"><span class="t">14:00</span><span class="n">Júlia P.</span><span class="d"></span></div>
                      <div class="fd-list-row"><span class="t">16:00</span><span class="n">Rafael T.</span><span class="d"></span></div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
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
  document.querySelectorAll('#fisioly .reveal').forEach(el => io.observe(el));
});
</script>
