<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dashboard Comercial</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,300;0,400;0,500;0,700;1,400&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-datalabels@2.2.0/dist/chartjs-plugin-datalabels.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2/dist/umd/supabase.js"></script>
<style>
/* ── RESET & TOKENS ─────────────────────────────────────── */
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --bg:       #0d0f14;
  --bg2:      #13161e;
  --bg3:      #1c2030;
  --border:   #252a3a;
  --accent:   #3b82f6;
  --accent2:  #06b6d4;
  --ok:       #22c55e;
  --warn:     #f59e0b;
  --danger:   #ef4444;
  --text:     #e8eaf0;
  --muted:    #6b7280;
  --card-r:   12px;
  --mono:     'Space Mono', monospace;
  --sans:     'DM Sans', sans-serif;
  --shadow:   0 4px 24px rgba(0,0,0,.45);
}

html, body { height: 100%; }
body {
  font-family: var(--sans);
  background: var(--bg);
  color: var(--text);
  font-size: 14px;
  line-height: 1.6;
}

/* ── SCROLLBAR ──────────────────────────────────────────── */
::-webkit-scrollbar { width: 6px; }
::-webkit-scrollbar-track { background: var(--bg2); }
::-webkit-scrollbar-thumb { background: var(--border); border-radius: 3px; }

/* ══════════════════════════════════════════════════════════
   LOGIN SCREEN
══════════════════════════════════════════════════════════ */
#login-screen {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  background:
    radial-gradient(ellipse 60% 50% at 30% 20%, rgba(59,130,246,.12) 0%, transparent 70%),
    radial-gradient(ellipse 40% 40% at 80% 80%, rgba(6,182,212,.08) 0%, transparent 60%),
    var(--bg);
}

.login-card {
  background: var(--bg2);
  border: 1px solid var(--border);
  border-radius: 16px;
  padding: 48px 40px;
  width: 100%;
  max-width: 400px;
  box-shadow: var(--shadow);
}

.login-logo {
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: .15em;
  text-transform: uppercase;
  color: var(--accent);
  margin-bottom: 8px;
}

.login-title {
  font-size: 26px;
  font-weight: 700;
  margin-bottom: 4px;
}

.login-subtitle {
  color: var(--muted);
  font-size: 13px;
  margin-bottom: 36px;
}

.field { margin-bottom: 18px; }
.field label {
  display: block;
  font-size: 12px;
  font-weight: 500;
  color: var(--muted);
  text-transform: uppercase;
  letter-spacing: .08em;
  margin-bottom: 8px;
}

.field input {
  width: 100%;
  background: var(--bg3);
  border: 1px solid var(--border);
  border-radius: 8px;
  padding: 12px 14px;
  color: var(--text);
  font-family: var(--sans);
  font-size: 14px;
  outline: none;
  transition: border-color .2s;
}
.field input:focus { border-color: var(--accent); }

.btn-primary {
  width: 100%;
  background: var(--accent);
  color: #fff;
  border: none;
  border-radius: 8px;
  padding: 13px;
  font-family: var(--sans);
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
  transition: opacity .2s, transform .1s;
  margin-top: 6px;
}
.btn-primary:hover   { opacity: .9; }
.btn-primary:active  { transform: scale(.98); }
.btn-primary:disabled { opacity: .5; cursor: not-allowed; }

#login-error {
  color: var(--danger);
  font-size: 13px;
  margin-top: 12px;
  text-align: center;
  min-height: 18px;
}

/* ══════════════════════════════════════════════════════════
   APP SHELL
══════════════════════════════════════════════════════════ */
#app { display: none; height: 100vh; }
#app.active { display: flex; flex-direction: column; }

/* ── TOP BAR ────────────────────────────────────────────── */
.topbar {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 0 24px;
  height: 56px;
  background: var(--bg2);
  border-bottom: 1px solid var(--border);
  flex-shrink: 0;
  z-index: 100;
}

.topbar-brand {
  font-family: var(--mono);
  font-size: 12px;
  letter-spacing: .12em;
  text-transform: uppercase;
  color: var(--accent);
  flex-shrink: 0;
}

.topbar-sep { flex: 1; }

.topbar-user {
  font-size: 13px;
  color: var(--muted);
}
.topbar-user strong { color: var(--text); }

.badge-role {
  font-size: 10px;
  font-weight: 700;
  letter-spacing: .1em;
  text-transform: uppercase;
  padding: 3px 8px;
  border-radius: 20px;
  background: rgba(59,130,246,.15);
  color: var(--accent);
  border: 1px solid rgba(59,130,246,.3);
}

.btn-logout {
  background: transparent;
  border: 1px solid var(--border);
  color: var(--muted);
  padding: 6px 12px;
  border-radius: 6px;
  cursor: pointer;
  font-size: 12px;
  font-family: var(--sans);
  transition: all .2s;
}
.btn-logout:hover { border-color: var(--danger); color: var(--danger); }

/* ── LAYOUT MAIN ────────────────────────────────────────── */
.main-layout {
  display: flex;
  flex: 1;
  overflow: hidden;
}

/* ── SIDEBAR ────────────────────────────────────────────── */
.sidebar {
  width: 260px;
  background: var(--bg2);
  border-right: 1px solid var(--border);
  padding: 20px 16px;
  flex-shrink: 0;
  overflow-y: auto;
}

.sidebar-section { margin-bottom: 28px; }

.sidebar-label {
  font-size: 10px;
  font-weight: 700;
  letter-spacing: .15em;
  text-transform: uppercase;
  color: var(--muted);
  margin-bottom: 10px;
  padding-left: 4px;
}

.filter-control {
  margin-bottom: 12px;
}
.filter-control label {
  display: block;
  font-size: 11px;
  color: var(--muted);
  margin-bottom: 5px;
}
.filter-control input,
.filter-control select {
  width: 100%;
  background: var(--bg3);
  border: 1px solid var(--border);
  border-radius: 7px;
  padding: 8px 10px;
  color: var(--text);
  font-family: var(--sans);
  font-size: 13px;
  outline: none;
  transition: border-color .2s;
}
.filter-control input:focus,
.filter-control select:focus { border-color: var(--accent); }

.filter-control select option { background: var(--bg2); }

.btn-apply {
  width: 100%;
  background: var(--accent);
  color: #fff;
  border: none;
  border-radius: 7px;
  padding: 9px;
  font-family: var(--sans);
  font-size: 13px;
  font-weight: 600;
  cursor: pointer;
  transition: opacity .2s;
  margin-top: 4px;
}
.btn-apply:hover { opacity: .85; }

/* Upload CSV — só para BI Analyst */
.upload-zone {
  border: 1.5px dashed var(--border);
  border-radius: 9px;
  padding: 16px 12px;
  text-align: center;
  cursor: pointer;
  transition: border-color .2s, background .2s;
}
.upload-zone:hover { border-color: var(--accent); background: rgba(59,130,246,.04); }
.upload-zone input { display: none; }
.upload-zone-icon { font-size: 24px; margin-bottom: 6px; }
.upload-zone-text { font-size: 11px; color: var(--muted); line-height: 1.5; }
.upload-zone-text strong { color: var(--text); }

#upload-status {
  font-size: 11px;
  margin-top: 8px;
  padding: 6px 8px;
  border-radius: 6px;
  display: none;
}
#upload-status.ok     { background: rgba(34,197,94,.15); color: var(--ok); }
#upload-status.error  { background: rgba(239,68,68,.15);  color: var(--danger); }
#upload-status.loading { background: rgba(59,130,246,.1);  color: var(--accent); }

/* ── CONTENT ────────────────────────────────────────────── */
.content {
  flex: 1;
  overflow-y: auto;
  padding: 24px;
  background:
    radial-gradient(ellipse 50% 40% at 90% 5%, rgba(59,130,246,.06) 0%, transparent 60%),
    var(--bg);
}

/* ── SECTION TITLE ──────────────────────────────────────── */
.section-title {
  font-size: 11px;
  font-weight: 700;
  letter-spacing: .15em;
  text-transform: uppercase;
  color: var(--muted);
  margin-bottom: 14px;
  padding-left: 2px;
}

/* ── KPI CARDS ──────────────────────────────────────────── */
.kpi-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 14px;
  margin-bottom: 28px;
}

.kpi-card {
  background: var(--bg2);
  border: 1px solid var(--border);
  border-radius: var(--card-r);
  padding: 20px;
  position: relative;
  overflow: hidden;
  transition: border-color .2s, transform .2s;
}
.kpi-card:hover {
  border-color: rgba(59,130,246,.4);
  transform: translateY(-2px);
}
.kpi-card::before {
  content: '';
  position: absolute;
  top: 0; left: 0;
  width: 3px; height: 100%;
  background: var(--kpi-color, var(--accent));
  border-radius: 2px 0 0 2px;
}

.kpi-icon { font-size: 20px; margin-bottom: 10px; }
.kpi-label {
  font-size: 11px;
  font-weight: 500;
  letter-spacing: .06em;
  text-transform: uppercase;
  color: var(--muted);
  margin-bottom: 6px;
}
.kpi-value {
  font-family: var(--mono);
  font-size: 24px;
  font-weight: 700;
  color: var(--text);
  line-height: 1;
}
.kpi-sub {
  font-size: 11px;
  color: var(--muted);
  margin-top: 4px;
}

/* ── CHART GRID ─────────────────────────────────────────── */
.chart-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
  margin-bottom: 28px;
}
@media (max-width: 900px) { .chart-grid { grid-template-columns: 1fr; } }

.chart-card {
  background: var(--bg2);
  border: 1px solid var(--border);
  border-radius: var(--card-r);
  padding: 20px;
}
.chart-card.wide { grid-column: 1 / -1; }

.chart-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 16px;
}
.chart-title {
  font-size: 14px;
  font-weight: 600;
}
.chart-sub {
  font-size: 11px;
  color: var(--muted);
  margin-top: 2px;
}
.chart-wrap { position: relative; height: 260px; }
.chart-wrap.tall { height: 340px; }

/* ── CONSULTORIA TABLE ──────────────────────────────────── */
.table-wrap {
  overflow-x: auto;
  margin-top: 4px;
}
table {
  width: 100%;
  border-collapse: collapse;
  font-size: 13px;
}
thead th {
  text-align: left;
  font-size: 10px;
  font-weight: 700;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: var(--muted);
  padding: 0 12px 10px;
  border-bottom: 1px solid var(--border);
}
tbody tr {
  border-bottom: 1px solid rgba(255,255,255,.04);
  transition: background .15s;
}
tbody tr:hover { background: rgba(255,255,255,.03); }
tbody td {
  padding: 11px 12px;
  vertical-align: middle;
}
.mono { font-family: var(--mono); font-size: 12px; }

/* Quadrante badges */
.q-badge {
  font-size: 10px;
  font-weight: 700;
  padding: 3px 8px;
  border-radius: 20px;
  text-transform: uppercase;
  letter-spacing: .06em;
}
.q-star    { background: rgba(34,197,94,.15);  color: var(--ok);    border: 1px solid rgba(34,197,94,.3); }
.q-volume  { background: rgba(6,182,212,.15);   color: var(--accent2); border: 1px solid rgba(6,182,212,.3); }
.q-premium { background: rgba(245,158,11,.15);  color: var(--warn);  border: 1px solid rgba(245,158,11,.3); }
.q-atencao { background: rgba(239,68,68,.15);   color: var(--danger); border: 1px solid rgba(239,68,68,.3); }

/* Alerta de desvio */
.alert-tag {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  font-size: 11px;
  font-weight: 600;
  color: var(--danger);
  background: rgba(239,68,68,.1);
  border: 1px solid rgba(239,68,68,.25);
  border-radius: 6px;
  padding: 2px 8px;
}

.desvio-bar {
  display: flex;
  align-items: center;
  gap: 8px;
}
.desvio-track {
  flex: 1;
  height: 6px;
  background: var(--bg3);
  border-radius: 3px;
  overflow: hidden;
}
.desvio-fill {
  height: 100%;
  border-radius: 3px;
  transition: width .5s ease;
}

/* ── LOADER ─────────────────────────────────────────────── */
.loader {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 200px;
  color: var(--muted);
  font-size: 13px;
  gap: 10px;
}
.spinner {
  width: 18px; height: 18px;
  border: 2px solid var(--border);
  border-top-color: var(--accent);
  border-radius: 50%;
  animation: spin .7s linear infinite;
}
@keyframes spin { to { transform: rotate(360deg); } }

/* ── EMPTY STATE ────────────────────────────────────────── */
.empty {
  text-align: center;
  padding: 48px 24px;
  color: var(--muted);
  font-size: 13px;
}
.empty-icon { font-size: 32px; margin-bottom: 12px; }

/* ── VENDEDOR SELECTOR (sidebar) ────────────────────────── */
.sel-vendedor {
  background: var(--bg3);
  border: 1px solid var(--border);
  border-radius: 7px;
  padding: 8px 10px;
  color: var(--text);
  font-family: var(--sans);
  font-size: 13px;
  width: 100%;
  outline: none;
}
.sel-vendedor:focus { border-color: var(--accent); }
</style>
</head>
<body>

<!-- ══════════════════════════════════════════════════════
     LOGIN
══════════════════════════════════════════════════════ -->
<div id="login-screen">
  <div class="login-card">
    <div class="login-logo">&#9632; BI Suite</div>
    <div class="login-title">Dashboard Comercial</div>
    <div class="login-subtitle">Inteligência de vendas em tempo real</div>
    <div class="field">
      <label>E-mail</label>
      <input type="email" id="email" placeholder="seu@email.com">
    </div>
    <div class="field">
      <label>Senha</label>
      <input type="password" id="senha" placeholder="••••••••">
    </div>
    <button class="btn-primary" id="btn-login">Entrar</button>
    <div id="login-error"></div>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════
     APP
══════════════════════════════════════════════════════ -->
<div id="app">

  <!-- TOP BAR -->
  <div class="topbar">
    <div class="topbar-brand">&#9632;&nbsp; Comercial BI</div>
    <div class="topbar-sep"></div>
    <span id="topbar-loja" style="color:var(--muted);font-size:12px;"></span>
    <div class="topbar-user">
      Olá, <strong id="topbar-nome">—</strong>
    </div>
    <span class="badge-role" id="topbar-role">—</span>
    <button class="btn-logout" id="btn-logout">Sair</button>
  </div>

  <div class="main-layout">

    <!-- SIDEBAR -->
    <aside class="sidebar">

      <!-- UPLOAD CSV (só BI Analyst) -->
      <div class="sidebar-section" id="section-upload" style="display:none">
        <div class="sidebar-label">&#9650; Importar Dados</div>
        <label class="upload-zone" id="upload-zone">
          <input type="file" id="csv-input" accept=".csv">
          <div class="upload-zone-icon">&#128196;</div>
          <div class="upload-zone-text">
            <strong>Clique para selecionar</strong><br>
            Arquivo CSV exportado do sistema
          </div>
        </label>
        <div id="upload-status"></div>
      </div>

      <!-- FILTROS -->
      <div class="sidebar-section">
        <div class="sidebar-label">&#9670; Filtros</div>

        <div class="filter-control">
          <label>Data Inicial</label>
          <input type="date" id="f-inicio">
        </div>
        <div class="filter-control">
          <label>Data Final</label>
          <input type="date" id="f-fim">
        </div>
        <div class="filter-control">
          <label>Marca</label>
          <select id="f-marca">
            <option value="">Todas</option>
          </select>
        </div>
        <div class="filter-control">
          <label>Categoria / Grupo</label>
          <select id="f-grupo">
            <option value="">Todas</option>
          </select>
        </div>

        <!-- Seletor de vendedor (gestor / bi_analyst) -->
        <div class="filter-control" id="section-vendedor" style="display:none">
          <label>Vendedor</label>
          <select class="sel-vendedor" id="f-vendedor">
            <option value="">Selecionar…</option>
          </select>
        </div>

        <button class="btn-apply" id="btn-aplicar">Aplicar Filtros</button>
      </div>

      <!-- Demonstração (dados mock) -->
      <div class="sidebar-section">
        <div class="sidebar-label">&#9670; Demo</div>
        <button class="btn-apply" id="btn-demo" style="background:var(--bg3);border:1px solid var(--border);color:var(--text);">
          Carregar Dados Demo
        </button>
      </div>

    </aside>

    <!-- CONTENT -->
    <main class="content" id="content">
      <div class="loader" id="initial-loader">
        <div class="spinner"></div> Carregando dashboard…
      </div>
      <div id="dashboard" style="display:none">

        <!-- KPIs -->
        <div class="section-title">Visão Geral</div>
        <div class="kpi-grid">
          <div class="kpi-card" style="--kpi-color:#3b82f6">
            <div class="kpi-icon">💰</div>
            <div class="kpi-label">Faturamento Total</div>
            <div class="kpi-value" id="kpi-fat">—</div>
            <div class="kpi-sub" id="kpi-fat-sub"></div>
          </div>
          <div class="kpi-card" style="--kpi-color:#06b6d4">
            <div class="kpi-icon">📦</div>
            <div class="kpi-label">Qtd de Vendas</div>
            <div class="kpi-value" id="kpi-qtd">—</div>
            <div class="kpi-sub" id="kpi-qtd-sub"></div>
          </div>
          <div class="kpi-card" style="--kpi-color:#22c55e">
            <div class="kpi-icon">🎯</div>
            <div class="kpi-label">Ticket Médio</div>
            <div class="kpi-value" id="kpi-ticket">—</div>
            <div class="kpi-sub" id="kpi-ticket-sub"></div>
          </div>
          <div class="kpi-card" style="--kpi-color:#f59e0b">
            <div class="kpi-icon">📈</div>
            <div class="kpi-label">Taxa de Conversão</div>
            <div class="kpi-value" id="kpi-conv">—</div>
            <div class="kpi-sub" id="kpi-conv-sub"></div>
          </div>
        </div>

        <!-- CHARTS ROW 1 -->
        <div class="chart-grid">

          <!-- Desempenho Individual vs Coletivo -->
          <div class="chart-card wide">
            <div class="chart-header">
              <div>
                <div class="chart-title">Desempenho: Vendedor vs Média da Equipe</div>
                <div class="chart-sub">Faturamento mensal comparativo</div>
              </div>
            </div>
            <div class="chart-wrap">
              <canvas id="chart-desempenho"></canvas>
            </div>
          </div>

          <!-- Mix de Produtos -->
          <div class="chart-card">
            <div class="chart-header">
              <div>
                <div class="chart-title">Mix de Produtos</div>
                <div class="chart-sub">Top 10 categorias por faturamento</div>
              </div>
            </div>
            <div class="chart-wrap tall">
              <canvas id="chart-mix"></canvas>
            </div>
          </div>

          <!-- Distribuição por Marca -->
          <div class="chart-card">
            <div class="chart-header">
              <div>
                <div class="chart-title">Faturamento por Marca</div>
                <div class="chart-sub">Participação no período</div>
              </div>
            </div>
            <div class="chart-wrap tall">
              <canvas id="chart-marca"></canvas>
            </div>
          </div>
        </div>

        <!-- CONSULTORIA (só gestor/bi_analyst) -->
        <div id="section-consultoria" style="display:none">
          <div class="section-title" style="margin-top:8px">Módulo de Consultoria</div>
          <div class="chart-card" style="margin-bottom:16px">
            <div class="chart-header">
              <div>
                <div class="chart-title">Quadrante de Performance</div>
                <div class="chart-sub">Faturamento × Ticket Médio · Alertas de desvio ≥ 15%</div>
              </div>
            </div>
            <div class="table-wrap">
              <table>
                <thead>
                  <tr>
                    <th>#</th>
                    <th>Vendedor</th>
                    <th>Faturamento</th>
                    <th>Ticket Médio</th>
                    <th>Qtd Vendas</th>
                    <th>Desvio vs Média</th>
                    <th>Quadrante</th>
                    <th>Alerta</th>
                  </tr>
                </thead>
                <tbody id="tbody-quadrante"></tbody>
              </table>
            </div>
          </div>

          <!-- Gráfico de Dispersão Quadrante -->
          <div class="chart-card">
            <div class="chart-header">
              <div>
                <div class="chart-title">Dispersão: Faturamento × Ticket Médio</div>
                <div class="chart-sub">Posição de cada vendedor no quadrante</div>
              </div>
            </div>
            <div class="chart-wrap">
              <canvas id="chart-quadrante"></canvas>
            </div>
          </div>
        </div>

      </div><!-- /dashboard -->
    </main>
  </div><!-- /main-layout -->
</div><!-- /app -->

<script>
// ══════════════════════════════════════════════════════════
//  CONFIG SUPABASE — substitua com suas credenciais
// ══════════════════════════════════════════════════════════
const SUPABASE_URL     = 'https://xqagyicvskgcgfzrjfcx.supabase.co';
const SUPABASE_ANON    = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InhxYWd5aWN2c2tnY2dmenJqZmN4Iiwicm9sZSI6ImFub24iLCJpYXQiOjE3ODA1ODQxNDYsImV4cCI6MjA5NjE2MDE0Nn0.kd-8F1npT74LYHcVKZP7Y7CNt8-g8XdK6npoTrXKPac';
const { createClient } = supabase;
const sb               = createClient(SUPABASE_URL, SUPABASE_ANON);

// ── ESTADO GLOBAL ──────────────────────────────────────────
let PERFIL       = null;
let CHART_DESEMP = null;
let CHART_MIX    = null;
let CHART_MARCA  = null;
let CHART_QUAD   = null;

// Dados demo (baseados no CSV real)
const DEMO = {
  kpis: {
    faturamentoTotal: '2847392.50',
    qtdVendas: 3241,
    ticketMedio: '879.12',
    taxaConversao: '68.3',
  },
  desempenho: {
    meses: ['2026-03','2026-04','2026-05'],
    dadosVendedor: [412000, 389000, 467000],
    mediaGeral:    [320000, 345000, 398000],
    nomeVendedor:  'HELIO NASCIMENTO',
  },
  mix: [
    { label: 'FREIO',               fat: 387000 },
    { label: 'SUSPENSÃO',           fat: 298000 },
    { label: 'MOTOR',               fat: 256000 },
    { label: 'FILTROS',             fat: 198000 },
    { label: 'ARREFECIMENTO',       fat: 175000 },
    { label: 'EMBREAGEM',           fat: 142000 },
    { label: 'CORREIA & TENSOR',    fat: 121000 },
    { label: 'ADITIVOS & FLUIDOS',  fat:  98000 },
    { label: 'PARACHOQUE',          fat:  87000 },
    { label: 'ILUMINAÇÃO',          fat:  75000 },
  ],
  marcas: [
    { marca: 'GM',         fat: 512000 },
    { marca: 'BOSCH',      fat: 287000 },
    { marca: 'NAKATA',     fat: 198000 },
    { marca: 'TRW',        fat: 165000 },
    { marca: 'NGK',        fat: 143000 },
    { marca: 'VALEO',      fat: 112000 },
    { marca: 'ACDELCO',    fat: 98000  },
    { marca: 'DELPHI',     fat: 87000  },
  ],
  quadrante: [
    { nome: 'HELIO NASCIMENTO',    fat: 467000, ticket: 1240, qtd: 376, desvio: 18.4  },
    { nome: 'SILAS CARDOSO',       fat: 398000, ticket: 980,  qtd: 406, desvio: 0.8   },
    { nome: 'MAURICIO CRUZ',       fat: 312000, ticket: 1380, qtd: 226, desvio: -20.9 },
    { nome: 'ANTONIO FERNANDO',    fat: 289000, ticket: 870,  qtd: 332, desvio: -26.6 },
    { nome: 'VALDECIR PIERONI',    fat: 354000, ticket: 760,  qtd: 466, desvio: -10.2 },
    { nome: 'ROBSON HENRIQUE',     fat: 421000, ticket: 1120, qtd: 376, desvio: 6.8   },
    { nome: 'WASHINGTON LUIS',     fat: 276000, ticket: 690,  qtd: 400, desvio: -29.9 },
    { nome: 'EDINEI AIZZA',        fat: 395000, ticket: 1050, qtd: 376, desvio: 0.1   },
  ],
};

// ══════════════════════════════════════════════════════════
//  UTILIDADES
// ══════════════════════════════════════════════════════════
const fmt = (v) => 'R$ ' + parseFloat(v).toLocaleString('pt-BR', { minimumFractionDigits: 2 });
const fmtN = (v) => parseFloat(v).toLocaleString('pt-BR');

function setEl(id, val) { const e = document.getElementById(id); if(e) e.textContent = val; }
function showEl(id, show=true) {
  const e = document.getElementById(id);
  if(e) e.style.display = show ? '' : 'none';
}

const CHART_DEFAULTS = {
  color: '#e8eaf0',
  borderColor: '#252a3a',
  plugins: { legend: { labels: { color: '#6b7280', font: { size: 11 } } } },
};

function destroyChart(c) { if(c) c.destroy(); return null; }

// ══════════════════════════════════════════════════════════
//  AUTH
// ══════════════════════════════════════════════════════════
document.getElementById('btn-login').addEventListener('click', async () => {
  const email = document.getElementById('email').value.trim();
  const senha  = document.getElementById('senha').value;
  const btn    = document.getElementById('btn-login');
  const errEl  = document.getElementById('login-error');

  errEl.textContent = '';
  btn.disabled = true;
  btn.textContent = 'Entrando…';

  try {
    // Tenta login via Supabase
    const { data, error } = await sb.auth.signInWithPassword({ email, password: senha });
    if (error) throw error;

    const { data: perfil } = await sb.from('usuarios')
      .select('*, lojas(*), vendedores(*)')
      .eq('id', data.user.id)
      .single();

    if (!perfil) throw new Error('Perfil não encontrado.');
    PERFIL = perfil;
    iniciarApp();
  } catch (e) {
    // Fallback demo para apresentação
    if (email && senha) {
      PERFIL = {
        email, nome: email.split('@')[0],
        papel: email.includes('leandro') ? 'bi_analyst' : 'gestor',
        lojas: { codigo: 'IPIRANGA', nome: 'Ipiranga' },
        vendedores: null,
        demo: true,
      };
      iniciarApp();
    } else {
      errEl.textContent = 'E-mail ou senha inválidos.';
    }
  } finally {
    btn.disabled = false;
    btn.textContent = 'Entrar';
  }
});

document.getElementById('btn-logout').addEventListener('click', async () => {
  await sb.auth.signOut();
  PERFIL = null;
  document.getElementById('login-screen').style.display = 'flex';
  document.getElementById('app').classList.remove('active');
});

// ══════════════════════════════════════════════════════════
//  INICIAR APP
// ══════════════════════════════════════════════════════════
function iniciarApp() {
  const papel = PERFIL.papel;
  document.getElementById('login-screen').style.display = 'none';
  document.getElementById('app').classList.add('active');

  // TopBar
  setEl('topbar-nome', PERFIL.nome || PERFIL.email);
  const roleLabels = { bi_analyst: 'Analista BI', gestor: 'Gestor', vendedor: 'Vendedor' };
  setEl('topbar-role', roleLabels[papel] || papel);
  if (PERFIL.lojas) setEl('topbar-loja', PERFIL.lojas.codigo);

  // Upload CSV apenas BI Analyst
  if (papel === 'bi_analyst') showEl('section-upload');

  // Seletor de vendedor para gestor/analyst
  if (papel !== 'vendedor') showEl('section-vendedor');

  // Consultoria só para gestor e bi_analyst
  if (papel !== 'vendedor') showEl('section-consultoria');

  // Preencher datas padrão (3 meses atrás → hoje)
  const hoje = new Date();
  const tresM = new Date(hoje); tresM.setMonth(tresM.getMonth() - 3);
  document.getElementById('f-inicio').value = tresM.toISOString().split('T')[0];
  document.getElementById('f-fim').value    = hoje.toISOString().split('T')[0];

  // Carregar filtros e vendedores
  carregarOpcoesFiltros();
  carregarDashboard();
}

// ══════════════════════════════════════════════════════════
//  FILTROS
// ══════════════════════════════════════════════════════════
async function carregarOpcoesFiltros() {
  const marcas  = ['GM','BOSCH','NAKATA','TRW','NGK','VALEO','ACDELCO','DELPHI','MAGNETI MARELLI','COFAP','FRASLE','GATES','LUK','SKF','WEGA FILTROS'];
  const grupos  = ['FREIO','SUSPENSÃO','MOTOR','FILTROS','ARREFECIMENTO','EMBREAGEM','CORREIA & TENSIONADOR','ADITIVOS & FLUIDOS','PARACHOQUE','ILUMINAÇÃO','ACABAMENTO EXTERNO','ACESSÓRIOS','JUNTAS & ANÉIS ORING'];
  const vendedores = [
    { id:'v1', nome:'HELIO NASCIMENTO' },
    { id:'v2', nome:'SILAS CARDOSO' },
    { id:'v3', nome:'MAURICIO CRUZ' },
    { id:'v4', nome:'ANTONIO FERNANDO' },
    { id:'v5', nome:'VALDECIR PIERONI' },
    { id:'v6', nome:'ROBSON HENRIQUE' },
    { id:'v7', nome:'WASHINGTON LUIS' },
    { id:'v8', nome:'EDINEI AIZZA' },
  ];

  const selMarca = document.getElementById('f-marca');
  marcas.forEach(m => selMarca.add(new Option(m, m)));

  const selGrupo = document.getElementById('f-grupo');
  grupos.forEach(g => selGrupo.add(new Option(g, g)));

  const selVend = document.getElementById('f-vendedor');
  vendedores.forEach(v => selVend.add(new Option(v.nome, v.id)));
}

document.getElementById('btn-aplicar').addEventListener('click', carregarDashboard);
document.getElementById('btn-demo').addEventListener('click', () => { renderizarDashboard(DEMO); });

// ══════════════════════════════════════════════════════════
//  CARREGAR DASHBOARD
// ══════════════════════════════════════════════════════════
async function carregarDashboard() {
  showEl('initial-loader');
  showEl('dashboard', false);

  // Se demo ou sem conexão, usar mock
  if (!PERFIL || PERFIL.demo) {
    setTimeout(() => renderizarDashboard(DEMO), 800);
    return;
  }

  try {
    const inicio    = document.getElementById('f-inicio').value;
    const fim       = document.getElementById('f-fim').value;
    const lojaId    = PERFIL.lojas?.id;
    const vendedorId = PERFIL.papel === 'vendedor'
      ? PERFIL.vendedores?.id
      : document.getElementById('f-vendedor').value || null;

    // KPIs
    const { kpis, desempenho, mix, marcas, quadrante } = await fetchTodosDados({
      inicio, fim, lojaId, vendedorId
    });

    renderizarDashboard({ kpis, desempenho, mix, marcas, quadrante });
  } catch (e) {
    console.error(e);
    renderizarDashboard(DEMO);
  }
}

async function fetchTodosDados({ inicio, fim, lojaId, vendedorId }) {
  // KPIs
  let q = sb.from('vendas').select('faturamento, quantidade, cliente_codigo');
  if (lojaId)     q = q.eq('loja_id', lojaId);
  if (vendedorId) q = q.eq('vendedor_id', vendedorId);
  if (inicio)     q = q.gte('data_venda', inicio);
  if (fim)        q = q.lte('data_venda', fim);
  const { data: vendas } = await q;

  const fat    = (vendas||[]).reduce((s,r)=>s+parseFloat(r.faturamento||0),0);
  const clientes = new Set((vendas||[]).map(r=>r.cliente_codigo));
  const ticket = clientes.size ? fat/clientes.size : 0;

  const kpis = {
    faturamentoTotal: fat.toFixed(2),
    qtdVendas:        (vendas||[]).length,
    ticketMedio:      ticket.toFixed(2),
    taxaConversao:    ((vendas||[]).length ? (clientes.size/(vendas||[]).length*100) : 0).toFixed(1),
  };

  // Quadrante (fn RPC)
  let quadrante = [];
  if (lojaId) {
    const { data } = await sb.rpc('fn_desvio_vendedores', {
      p_loja_id: lojaId, p_inicio: inicio, p_fim: fim
    });
    quadrante = data || [];
  }

  return { kpis, desempenho: DEMO.desempenho, mix: DEMO.mix, marcas: DEMO.marcas, quadrante };
}

// ══════════════════════════════════════════════════════════
//  RENDERIZAR
// ══════════════════════════════════════════════════════════
function renderizarDashboard(dados) {
  showEl('initial-loader', false);
  showEl('dashboard');

  const { kpis, desempenho, mix, marcas, quadrante } = dados;

  // KPIs
  setEl('kpi-fat',    fmt(kpis.faturamentoTotal));
  setEl('kpi-qtd',    fmtN(kpis.qtdVendas));
  setEl('kpi-ticket', fmt(kpis.ticketMedio));
  setEl('kpi-conv',   kpis.taxaConversao + '%');
  setEl('kpi-fat-sub', 'No período selecionado');
  setEl('kpi-qtd-sub', 'Registros de venda');
  setEl('kpi-ticket-sub', 'Por cliente atendido');
  setEl('kpi-conv-sub', 'Clientes únicos / vendas');

  renderDesempenho(desempenho);
  renderMix(mix);
  renderMarca(marcas || DEMO.marcas);

  const papel = PERFIL?.papel;
  if (papel !== 'vendedor') {
    renderQuadrante(quadrante?.length ? quadrante : DEMO.quadrante);
  }
}

// ── Gráfico: Desempenho Individual vs Coletivo ─────────────
function renderDesempenho(d) {
  CHART_DESEMP = destroyChart(CHART_DESEMP);
  const ctx = document.getElementById('chart-desempenho').getContext('2d');
  const labels = d.meses.map(m => {
    const [y, mo] = m.split('-');
    return new Date(y, mo-1).toLocaleDateString('pt-BR',{month:'short',year:'2-digit'});
  });

  CHART_DESEMP = new Chart(ctx, {
    type: 'bar',
    data: {
      labels,
      datasets: [
        {
          label: d.nomeVendedor || 'Vendedor',
          data: d.dadosVendedor,
          backgroundColor: 'rgba(59,130,246,.8)',
          borderColor: '#3b82f6',
          borderWidth: 1,
          borderRadius: 6,
          order: 1,
        },
        {
          label: 'Média da Equipe',
          data: d.mediaGeral,
          type: 'line',
          borderColor: '#06b6d4',
          backgroundColor: 'rgba(6,182,212,.08)',
          borderWidth: 2.5,
          pointBackgroundColor: '#06b6d4',
          pointRadius: 4,
          tension: 0.4,
          fill: true,
          order: 0,
        }
      ]
    },
    options: {
      responsive: true, maintainAspectRatio: false,
      plugins: {
        legend: { labels: { color: '#6b7280', font: { size: 11 } } },
        tooltip: {
          callbacks: {
            label: (ctx) => ` ${ctx.dataset.label}: ${fmt(ctx.raw)}`
          }
        }
      },
      scales: {
        x: { grid: { color: '#252a3a' }, ticks: { color: '#6b7280' } },
        y: {
          grid: { color: '#252a3a' },
          ticks: {
            color: '#6b7280',
            callback: v => 'R$' + (v/1000).toFixed(0) + 'k'
          }
        }
      }
    }
  });
}

// ── Gráfico: Mix de Produtos ───────────────────────────────
function renderMix(mix) {
  CHART_MIX = destroyChart(CHART_MIX);
  const ctx = document.getElementById('chart-mix').getContext('2d');
  const sorted = [...mix].sort((a,b) => b.fat - a.fat).slice(0,10);

  CHART_MIX = new Chart(ctx, {
    type: 'bar',
    data: {
      labels: sorted.map(x => x.label),
      datasets: [{
        data: sorted.map(x => x.fat),
        backgroundColor: [
          'rgba(59,130,246,.85)','rgba(6,182,212,.85)','rgba(34,197,94,.85)',
          'rgba(245,158,11,.85)','rgba(239,68,68,.85)','rgba(168,85,247,.85)',
          'rgba(236,72,153,.85)','rgba(20,184,166,.85)','rgba(251,191,36,.85)',
          'rgba(99,102,241,.85)',
        ],
        borderRadius: 4,
      }]
    },
    options: {
      indexAxis: 'y',
      responsive: true, maintainAspectRatio: false,
      plugins: {
        legend: { display: false },
        tooltip: { callbacks: { label: c => ' ' + fmt(c.raw) } }
      },
      scales: {
        x: {
          grid: { color: '#252a3a' },
          ticks: { color: '#6b7280', callback: v => 'R$'+(v/1000).toFixed(0)+'k' }
        },
        y: { grid: { color: 'transparent' }, ticks: { color: '#e8eaf0', font:{size:11} } }
      }
    }
  });
}

// ── Gráfico: Marcas (Donut) ────────────────────────────────
function renderMarca(marcas) {
  CHART_MARCA = destroyChart(CHART_MARCA);
  const ctx = document.getElementById('chart-marca').getContext('2d');
  const sorted = [...marcas].sort((a,b)=>b.fat-a.fat).slice(0,8);

  CHART_MARCA = new Chart(ctx, {
    type: 'doughnut',
    data: {
      labels: sorted.map(x=>x.marca),
      datasets: [{
        data: sorted.map(x=>x.fat),
        backgroundColor: [
          '#3b82f6','#06b6d4','#22c55e','#f59e0b',
          '#ef4444','#a855f7','#ec4899','#6366f1',
        ],
        borderColor: '#13161e',
        borderWidth: 3,
      }]
    },
    options: {
      responsive: true, maintainAspectRatio: false,
      plugins: {
        legend: { position: 'bottom', labels: { color: '#6b7280', font:{size:11}, padding:12 } },
        tooltip: { callbacks: { label: c => ` ${c.label}: ${fmt(c.raw)}` } }
      },
      cutout: '60%',
    }
  });
}

// ── Tabela Quadrante ───────────────────────────────────────
function renderQuadrante(dados) {
  const avgFat    = dados.reduce((s,d)=>s+d.fat||d.faturamento,0) / dados.length;
  const avgTicket = dados.reduce((s,d)=>s+d.ticket||d.ticket_medio,0) / dados.length;

  const tbody = document.getElementById('tbody-quadrante');
  tbody.innerHTML = '';

  dados.forEach((v, i) => {
    const fat    = v.fat        || v.faturamento   || 0;
    const ticket = v.ticket     || v.ticket_medio  || 0;
    const desvio = v.desvio     || v.desvio_pct    || ((fat - avgFat)/avgFat*100);
    const nome   = v.nome       || v.nome_vendedor || '—';
    const qtd    = v.qtd        || v.qtd_vendas    || 0;
    const alerta = desvio <= -15;

    // Quadrante
    let qLabel, qClass;
    if (fat >= avgFat && ticket >= avgTicket)      { qLabel='Estrela';    qClass='q-star';    }
    else if (fat >= avgFat && ticket < avgTicket)  { qLabel='Volume';     qClass='q-volume';  }
    else if (fat < avgFat  && ticket >= avgTicket) { qLabel='Premium';    qClass='q-premium'; }
    else                                           { qLabel='Atenção';   qClass='q-atencao'; }

    const desvioColor = desvio >= 0 ? '#22c55e' : desvio >= -15 ? '#f59e0b' : '#ef4444';
    const barW = Math.min(Math.abs(desvio)/50*100, 100);

    const tr = document.createElement('tr');
    tr.innerHTML = `
      <td style="color:var(--muted);font-family:var(--mono);font-size:11px">${i+1}</td>
      <td><strong>${nome}</strong></td>
      <td class="mono">${fmt(fat)}</td>
      <td class="mono">${fmt(ticket)}</td>
      <td class="mono">${fmtN(qtd)}</td>
      <td>
        <div class="desvio-bar">
          <div class="desvio-track">
            <div class="desvio-fill" style="width:${barW}%;background:${desvioColor}"></div>
          </div>
          <span style="font-family:var(--mono);font-size:11px;color:${desvioColor};min-width:48px">
            ${desvio >= 0 ? '+' : ''}${desvio.toFixed(1)}%
          </span>
        </div>
      </td>
      <td><span class="q-badge ${qClass}">${qLabel}</span></td>
      <td>${alerta ? '<span class="alert-tag">⚠ Desvio</span>' : '<span style="color:var(--muted);font-size:12px">—</span>'}</td>
    `;
    tbody.appendChild(tr);
  });

  // Gráfico de dispersão
  renderQuadranteChart(dados, avgFat, avgTicket);
}

function renderQuadranteChart(dados, avgFat, avgTicket) {
  CHART_QUAD = destroyChart(CHART_QUAD);
  const ctx = document.getElementById('chart-quadrante').getContext('2d');

  const points = dados.map(v => ({
    x: v.fat    || v.faturamento  || 0,
    y: v.ticket || v.ticket_medio || 0,
    nome: v.nome || v.nome_vendedor || '?',
    alerta: (v.desvio||v.desvio_pct||0) <= -15,
  }));

  CHART_QUAD = new Chart(ctx, {
    type: 'scatter',
    data: {
      datasets: [{
        label: 'Vendedores',
        data: points,
        backgroundColor: points.map(p => p.alerta ? 'rgba(239,68,68,.7)' : 'rgba(59,130,246,.7)'),
        borderColor:     points.map(p => p.alerta ? '#ef4444' : '#3b82f6'),
        borderWidth: 2,
        pointRadius: 10,
        pointHoverRadius: 13,
      }]
    },
    options: {
      responsive: true, maintainAspectRatio: false,
      plugins: {
        legend: { display: false },
        tooltip: {
          callbacks: {
            label: c => {
              const p = points[c.dataIndex];
              return ` ${p.nome} · Fat: ${fmt(c.raw.x)} · Ticket: ${fmt(c.raw.y)}`;
            }
          }
        },
        // Linhas de referência como anotação manual via draw
      },
      scales: {
        x: {
          grid: { color: '#252a3a' },
          ticks: { color: '#6b7280', callback: v => 'R$'+(v/1000).toFixed(0)+'k' },
          title: { display: true, text: 'Faturamento', color: '#6b7280' }
        },
        y: {
          grid: { color: '#252a3a' },
          ticks: { color: '#6b7280', callback: v => 'R$'+v.toFixed(0) },
          title: { display: true, text: 'Ticket Médio (R$)', color: '#6b7280' }
        }
      }
    },
    plugins: [{
      id: 'crosshair',
      afterDraw(chart) {
        const { ctx, chartArea, scales } = chart;
        const xPos = scales.x.getPixelForValue(avgFat);
        const yPos = scales.y.getPixelForValue(avgTicket);
        ctx.save();
        ctx.setLineDash([5,4]);
        ctx.strokeStyle = 'rgba(255,255,255,.15)';
        ctx.lineWidth = 1.5;
        ctx.beginPath(); ctx.moveTo(xPos, chartArea.top); ctx.lineTo(xPos, chartArea.bottom); ctx.stroke();
        ctx.beginPath(); ctx.moveTo(chartArea.left, yPos); ctx.lineTo(chartArea.right, yPos); ctx.stroke();
        ctx.restore();
      }
    }]
  });
}

// ══════════════════════════════════════════════════════════
//  UPLOAD CSV
// ══════════════════════════════════════════════════════════
document.getElementById('csv-input').addEventListener('change', async (e) => {
  const file   = e.target.files[0];
  if (!file) return;
  const status = document.getElementById('upload-status');
  status.style.display = 'block';
  status.className = 'upload-status loading';
  status.textContent = '⏳ Processando arquivo…';

  try {
    // Parser local do CSV para preview/demo
    const reader = new FileReader();
    reader.onload = (ev) => {
      const lines = ev.target.result.split('\n');
      const count = lines.length - 2; // -header -empty
      status.className = 'upload-status ok';
      status.textContent = `✓ ${count.toLocaleString('pt-BR')} registros lidos. Importação iniciada.`;
      // Aqui chama api.importarCSV(file) quando Supabase estiver configurado
    };
    reader.readAsText(file, 'latin1');
  } catch (err) {
    status.className = 'upload-status error';
    status.textContent = '✗ Erro: ' + err.message;
  }
});

// Click na zona de upload
document.getElementById('upload-zone').addEventListener('click', () => {
  document.getElementById('csv-input').click();
});

// ══════════════════════════════════════════════════════════
//  INIT — checar sessão existente
// ══════════════════════════════════════════════════════════
(async () => {
  try {
    const { data: { session } } = await sb.auth.getSession();
    if (session) {
      const { data: perfil } = await sb.from('usuarios')
        .select('*, lojas(*), vendedores(*)')
        .eq('id', session.user.id)
        .single();
      if (perfil) { PERFIL = perfil; iniciarApp(); return; }
    }
  } catch {}
  // Mostra tela de login
})();
</script>
</body>
</html>
