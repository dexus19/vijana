<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>UMOJA WVJ — Group Manager</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
:root {
  --bg:#f5f2ec; --surface:#fff; --surface2:#f0ede6; --border:#ddd9d0;
  --primary:#0f5c4a; --primary-light:#e8f5f1; --primary-mid:#1a7a63;
  --accent:#e8860a; --danger:#c0392b; --danger-light:#fdecea;
  --text:#1a1a18; --text2:#5a5a52; --text3:#9a9a90; --gold:#c9920a;
  --paid:#0f5c4a; --paid-bg:#e8f5f1;
  --unpaid-bg:#f0ede6;
  --shadow:0 2px 16px rgba(15,92,74,.08);
  --shadow-lg:0 8px 40px rgba(15,92,74,.15);
  --rl:16px; --sidebar-w:220px; --topbar-h:56px; --bottom-nav-h:64px;
}
*{box-sizing:border-box;margin:0;padding:0}
html,body{height:100%}
body{font-family:'Plus Jakarta Sans',sans-serif;background:var(--bg);color:var(--text);font-size:14px;-webkit-tap-highlight-color:transparent}

/* ── Layout ── */
.app{display:flex;min-height:100vh}

/* ── Sidebar ── */
.sidebar{width:var(--sidebar-w);background:var(--primary);display:flex;flex-direction:column;position:fixed;top:0;left:0;bottom:0;z-index:300;transition:transform .25s cubic-bezier(.4,0,.2,1)}
.sidebar-logo{padding:22px 20px 14px;border-bottom:1px solid rgba(255,255,255,.1)}
.sidebar-logo .org-tag{font-size:9px;letter-spacing:.18em;text-transform:uppercase;color:rgba(255,255,255,.5);margin-bottom:4px}
.sidebar-logo h1{font-size:15px;font-weight:800;color:#fff;line-height:1.2}
.sidebar-logo .group-type{font-size:10px;color:rgba(255,255,255,.4);margin-top:2px;font-family:'DM Mono',monospace}
nav{padding:14px 0;flex:1}
.nav-item{display:flex;align-items:center;gap:10px;padding:10px 20px;color:rgba(255,255,255,.65);cursor:pointer;font-size:13px;font-weight:500;border-left:3px solid transparent;transition:all .15s;user-select:none}
.nav-item:hover{background:rgba(255,255,255,.07);color:#fff}
.nav-item.active{background:rgba(255,255,255,.1);color:#fff;border-left-color:#7ddbbb}
.nav-item .icon{font-size:16px;width:20px;text-align:center}
.sidebar-footer{padding:14px 20px;border-top:1px solid rgba(255,255,255,.1);font-size:10px;color:rgba(255,255,255,.3);font-family:'DM Mono',monospace}
.sidebar-overlay{display:none;position:fixed;inset:0;background:rgba(0,0,0,.45);z-index:299}
.sidebar-overlay.open{display:block}

/* ── Main ── */
.main{margin-left:var(--sidebar-w);flex:1;min-height:100vh;display:flex;flex-direction:column}
.topbar{background:var(--surface);border-bottom:1px solid var(--border);padding:0 20px;height:var(--topbar-h);display:flex;align-items:center;justify-content:space-between;position:sticky;top:0;z-index:50;gap:12px}
.topbar-left{display:flex;align-items:center;gap:10px;min-width:0}
.hamburger{display:none;background:none;border:none;cursor:pointer;padding:6px;border-radius:8px;color:var(--text);flex-shrink:0}
.hamburger:hover{background:var(--surface2)}
.topbar-title{font-size:15px;font-weight:700;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.topbar-sub{font-size:11px;color:var(--text3);font-family:'DM Mono',monospace;white-space:nowrap}
.topbar-actions{display:flex;gap:8px;align-items:center;flex-shrink:0}
.content{padding:20px 24px;flex:1}
.view{display:none}.view.active{display:block}

/* ── Buttons ── */
.btn{display:inline-flex;align-items:center;gap:6px;padding:8px 16px;border-radius:8px;font-family:'Plus Jakarta Sans',sans-serif;font-size:13px;font-weight:600;cursor:pointer;border:none;transition:all .15s;white-space:nowrap}
.btn-primary{background:var(--primary);color:#fff}.btn-primary:hover{background:var(--primary-mid)}
.btn-accent{background:var(--accent);color:#fff}.btn-accent:hover{background:#c97309}
.btn-export{background:#1d4ed8;color:#fff}.btn-export:hover{background:#1e40af}
.btn-ghost{background:transparent;color:var(--text2);border:1px solid var(--border)}.btn-ghost:hover{background:var(--surface2)}
.btn-danger{background:var(--danger-light);color:var(--danger);border:1px solid #f5c6c2}.btn-danger:hover{background:#f9d5d2}
.btn-sm{padding:5px 10px;font-size:12px}.btn-icon{padding:7px}

/* Export */
.export-wrap{position:relative;display:inline-block}
.export-menu{display:none;position:absolute;right:0;top:calc(100% + 4px);background:var(--surface);border:1px solid var(--border);border-radius:10px;box-shadow:var(--shadow-lg);min-width:160px;z-index:200;overflow:hidden}
.export-menu.open{display:block}
.export-item{display:flex;align-items:center;gap:8px;padding:10px 14px;font-size:13px;font-weight:500;cursor:pointer;color:var(--text);transition:background .1s}
.export-item:hover{background:var(--surface2)}

/* FAB */
.fab{display:none;position:fixed;bottom:calc(var(--bottom-nav-h) + 16px);right:18px;width:52px;height:52px;border-radius:50%;background:var(--primary);color:#fff;font-size:24px;border:none;cursor:pointer;box-shadow:0 4px 20px rgba(15,92,74,.35);align-items:center;justify-content:center;z-index:100;transition:transform .15s}
.fab:active{transform:scale(.93)}

/* Bottom nav */
.bottom-nav{display:none;position:fixed;bottom:0;left:0;right:0;height:var(--bottom-nav-h);background:var(--primary);z-index:200;border-top:1px solid rgba(255,255,255,.12)}
.bottom-nav-inner{display:flex;height:100%}
.bnav-item{flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:3px;cursor:pointer;color:rgba(255,255,255,.55);transition:color .15s,background .15s;font-size:10px;font-weight:600;letter-spacing:.04em;text-transform:uppercase;border:none;background:transparent}
.bnav-item .bnav-icon{font-size:20px;line-height:1}
.bnav-item.active{color:#fff;background:rgba(255,255,255,.1)}
.bnav-item:active{background:rgba(255,255,255,.15)}

/* ── Stats ── */
.stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:24px}
.stat-card{background:var(--surface);border:1px solid var(--border);border-radius:var(--rl);padding:18px 16px;box-shadow:var(--shadow);position:relative;overflow:hidden}
.stat-card::before{content:'';position:absolute;top:0;left:0;right:0;height:3px}
.stat-card.green::before{background:var(--primary)}.stat-card.amber::before{background:var(--accent)}.stat-card.blue::before{background:#2563eb}.stat-card.red::before{background:var(--danger)}
.stat-icon{font-size:20px;margin-bottom:8px}
.stat-value{font-size:22px;font-weight:800;line-height:1;font-family:'DM Mono',monospace}
.stat-label{font-size:10px;color:var(--text3);margin-top:4px;text-transform:uppercase;letter-spacing:.08em;font-weight:600}
.stat-sub{font-size:11px;color:var(--text2);margin-top:4px;font-family:'DM Mono',monospace}

/* ── Dashboard ── */
.dash-grid{display:grid;grid-template-columns:1fr 300px;gap:18px}
.card{background:var(--surface);border:1px solid var(--border);border-radius:var(--rl);box-shadow:var(--shadow);overflow:hidden}
.card-header{padding:14px 18px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between}
.card-title{font-size:12px;font-weight:700;text-transform:uppercase;letter-spacing:.07em}
.payment-list{list-style:none}
.payment-item{display:flex;align-items:center;padding:10px 18px;border-bottom:1px solid var(--border);gap:10px;transition:background .1s}
.payment-item:last-child{border-bottom:none}
.payment-item:hover{background:var(--surface2)}
.member-avatar{width:32px;height:32px;border-radius:50%;background:var(--primary-light);color:var(--primary);font-size:11px;font-weight:700;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.payment-name{font-size:13px;font-weight:600;flex:1;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.payment-deposit{font-size:11px;font-family:'DM Mono',monospace;color:var(--text2);flex-shrink:0}
.status-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0}
.dot-paid{background:var(--paid)}.dot-partial{background:var(--accent)}.dot-unpaid{background:#ddd}
.month-progress{padding:12px 18px}
.month-row{display:flex;align-items:center;gap:8px;margin-bottom:7px}
.month-label{font-size:10px;font-weight:600;width:36px;color:var(--text2);flex-shrink:0}
.progress-bar{flex:1;height:5px;background:var(--surface2);border-radius:4px;overflow:hidden}
.progress-fill{height:100%;border-radius:4px;background:var(--primary);transition:width .5s ease}
.progress-fill.partial{background:var(--accent)}
.month-pct{font-size:10px;color:var(--text3);font-family:'DM Mono',monospace;width:28px;text-align:right}

/* ── Table ── */
.table-controls{display:flex;align-items:center;gap:10px;margin-bottom:14px;flex-wrap:wrap}
.search-box{display:flex;align-items:center;gap:8px;background:var(--surface);border:1px solid var(--border);border-radius:8px;padding:8px 12px;flex:1;min-width:0}
.search-box input{border:none;outline:none;font-family:'Plus Jakarta Sans',sans-serif;font-size:13px;color:var(--text);background:transparent;width:100%}
.search-box input::placeholder{color:var(--text3)}
select.filter-sel{padding:8px 10px;border:1px solid var(--border);border-radius:8px;font-family:'Plus Jakarta Sans',sans-serif;font-size:13px;background:var(--surface);color:var(--text);outline:none;cursor:pointer}
.table-wrap{background:var(--surface);border:1px solid var(--border);border-radius:var(--rl);box-shadow:var(--shadow);overflow:hidden}
.table-scroll{overflow-x:auto;-webkit-overflow-scrolling:touch}
table{width:100%;border-collapse:collapse}
thead tr{background:var(--surface2);border-bottom:2px solid var(--border)}
th{padding:10px 12px;text-align:left;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.1em;color:var(--text3);white-space:nowrap}
th.center,td.center{text-align:center}
th.right,td.right{text-align:right}
tbody tr{border-bottom:1px solid var(--border);transition:background .1s;cursor:pointer}
tbody tr:last-child{border-bottom:none}
tbody tr:hover{background:var(--surface2)}
td{padding:9px 12px;vertical-align:middle}
.member-name-cell{display:flex;align-items:center;gap:10px}
.member-name{font-weight:600;font-size:13px}
.member-phone{font-size:11px;color:var(--text3);font-family:'DM Mono',monospace}
.role-pill{font-size:9px;font-weight:700;padding:2px 6px;border-radius:4px;text-transform:uppercase;letter-spacing:.06em}
.role-chair{background:#fef3e2;color:var(--gold)}
.role-treasurer{background:var(--primary-light);color:var(--primary)}
.role-member{background:var(--surface2);color:var(--text3)}
.amount-cell{font-family:'DM Mono',monospace;font-size:13px;font-weight:500;color:var(--primary)}
.amount-zero{color:var(--text3);font-family:'DM Mono',monospace}
.pay-pill{display:inline-block;font-size:10px;font-family:'DM Mono',monospace;padding:2px 6px;border-radius:5px;min-width:50px;text-align:center;font-weight:500;white-space:nowrap}
.pay-paid{background:var(--paid-bg);color:var(--paid)}
.pay-unpaid{background:var(--unpaid-bg);color:var(--text3)}
.action-btns{display:flex;gap:4px;justify-content:center}
.sticky-col{position:sticky;left:0;background:var(--surface);z-index:2}
tbody tr:hover .sticky-col{background:var(--surface2)}
tfoot tr{background:var(--surface2);border-top:2px solid var(--border)}
tfoot td{font-size:12px;font-weight:700;padding:9px 12px;font-family:'DM Mono',monospace;color:var(--primary)}
tfoot td.label-cell{font-family:'Plus Jakarta Sans',sans-serif;font-size:11px;text-transform:uppercase;letter-spacing:.08em;color:var(--text3)}

/* ── Member cards (mobile) ── */
.member-cards{display:none;flex-direction:column;gap:10px}
.member-card{background:var(--surface);border:1px solid var(--border);border-radius:var(--rl);box-shadow:var(--shadow);overflow:hidden;cursor:pointer}
.member-card:active{box-shadow:none}
.member-card-top{display:flex;align-items:center;gap:12px;padding:14px 16px}
.mc-avatar{width:40px;height:40px;border-radius:12px;background:var(--primary-light);color:var(--primary);font-size:14px;font-weight:700;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.mc-info{flex:1;min-width:0}
.mc-name{font-weight:700;font-size:14px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.mc-phone{font-size:11px;color:var(--text3);font-family:'DM Mono',monospace;margin-top:1px}
.mc-deposit{text-align:right;flex-shrink:0}
.mc-dep-val{font-size:15px;font-weight:800;font-family:'DM Mono',monospace;color:var(--primary)}
.mc-dep-val.zero{color:var(--text3)}
.mc-dep-label{font-size:9px;color:var(--text3);text-transform:uppercase;letter-spacing:.08em;margin-top:1px;text-align:right}
.member-card-pills{display:flex;gap:6px;padding:0 16px 10px;flex-wrap:wrap;align-items:center;border-top:1px solid var(--border);padding-top:10px}
.mc-role{margin-right:auto}
.member-card-actions{display:flex;gap:8px;padding:0 16px 14px}
.member-card-actions .btn{flex:1;justify-content:center}

/* ═══════════════════════════════
   EVENTS PAGE
═══════════════════════════════ */

/* Event list grid */
.events-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:18px;gap:12px;flex-wrap:wrap}
.events-header-left h2{font-size:18px;font-weight:800}
.events-header-left p{font-size:12px;color:var(--text3);margin-top:2px;font-family:'DM Mono',monospace}

.events-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(300px,1fr));gap:16px}

.event-card{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--rl);
  box-shadow:var(--shadow);overflow:hidden;cursor:pointer;
  transition:box-shadow .15s,transform .15s;
}
.event-card:hover{box-shadow:var(--shadow-lg);transform:translateY(-2px)}
.event-card:active{transform:translateY(0);box-shadow:var(--shadow)}

.event-card-banner{
  height:6px;
  background:linear-gradient(90deg,var(--primary),var(--primary-mid));
}
.event-card-body{padding:16px}
.event-card-top{display:flex;align-items:flex-start;justify-content:space-between;gap:8px;margin-bottom:10px}
.event-name{font-size:15px;font-weight:800;line-height:1.2}
.event-date-badge{
  font-size:10px;font-family:'DM Mono',monospace;font-weight:500;
  background:var(--primary-light);color:var(--primary);
  padding:3px 8px;border-radius:5px;white-space:nowrap;flex-shrink:0;
}
.event-desc{font-size:12px;color:var(--text3);margin-bottom:12px;line-height:1.5;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden}
.event-amount-row{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px}
.event-amount-label{font-size:11px;color:var(--text2);font-weight:600}
.event-amount-val{font-size:16px;font-weight:800;font-family:'DM Mono',monospace;color:var(--primary)}

/* Progress ring area */
.event-progress-row{display:flex;align-items:center;gap:10px;margin-bottom:14px}
.event-prog-bar-wrap{flex:1}
.event-prog-bar{height:7px;background:var(--surface2);border-radius:4px;overflow:hidden}
.event-prog-fill{height:100%;border-radius:4px;background:var(--primary);transition:width .5s ease}
.event-prog-label{font-size:11px;font-family:'DM Mono',monospace;color:var(--text3);white-space:nowrap}

.event-counters{display:flex;gap:8px}
.ev-counter{flex:1;text-align:center;background:var(--surface2);border-radius:8px;padding:8px 4px}
.ev-counter-val{font-size:16px;font-weight:800;font-family:'DM Mono',monospace}
.ev-counter-label{font-size:9px;color:var(--text3);text-transform:uppercase;letter-spacing:.07em;margin-top:2px}
.ev-counter.paid .ev-counter-val{color:var(--paid)}
.ev-counter.unpaid .ev-counter-val{color:var(--danger)}
.ev-counter.total .ev-counter-val{color:var(--text2)}

.event-card-footer{
  padding:10px 16px;border-top:1px solid var(--border);
  display:flex;gap:6px;align-items:center;
}

/* Empty events */
.events-empty{
  text-align:center;padding:60px 20px;color:var(--text3);
  background:var(--surface);border:2px dashed var(--border);border-radius:var(--rl);
}
.events-empty .icon{font-size:40px;margin-bottom:12px}
.events-empty h3{font-size:16px;font-weight:700;color:var(--text2);margin-bottom:6px}
.events-empty p{font-size:13px}

/* ── Event Detail Page ── */
.event-detail-page{display:none}
.event-detail-page.active{display:block}

.back-btn{display:inline-flex;align-items:center;gap:6px;font-size:13px;font-weight:600;color:var(--primary);cursor:pointer;margin-bottom:18px;padding:6px 0}
.back-btn:hover{opacity:.75}

.event-detail-hero{
  background:var(--surface);border:1px solid var(--border);border-radius:var(--rl);
  box-shadow:var(--shadow);margin-bottom:20px;overflow:hidden;
}
.event-detail-hero-banner{height:8px;background:linear-gradient(90deg,var(--primary),var(--primary-mid))}
.event-detail-hero-body{padding:20px 24px}
.event-detail-top{display:flex;align-items:flex-start;justify-content:space-between;gap:12px;margin-bottom:16px;flex-wrap:wrap}
.event-detail-name{font-size:22px;font-weight:800}
.event-detail-meta{display:flex;gap:8px;flex-wrap:wrap;margin-top:6px}
.meta-badge{font-size:11px;font-family:'DM Mono',monospace;padding:3px 10px;border-radius:5px;font-weight:500}
.meta-date{background:var(--primary-light);color:var(--primary)}
.meta-amount{background:#fef3e2;color:var(--accent)}
.event-detail-desc{font-size:13px;color:var(--text2);margin-bottom:18px;line-height:1.6}
.event-detail-stats{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
.eds-card{background:var(--surface2);border-radius:10px;padding:14px;text-align:center}
.eds-val{font-size:22px;font-weight:800;font-family:'DM Mono',monospace}
.eds-label{font-size:10px;text-transform:uppercase;letter-spacing:.08em;color:var(--text3);margin-top:3px;font-weight:600}
.eds-card.paid .eds-val{color:var(--paid)}
.eds-card.unpaid .eds-val{color:var(--danger)}
.eds-card.total .eds-val{color:var(--text2)}

/* Member contribution table */
.contrib-section-title{font-size:13px;font-weight:700;text-transform:uppercase;letter-spacing:.08em;color:var(--text3);margin-bottom:12px;margin-top:4px}

.contrib-table-wrap{background:var(--surface);border:1px solid var(--border);border-radius:var(--rl);box-shadow:var(--shadow);overflow:hidden}
.contrib-row{display:flex;align-items:center;padding:12px 18px;border-bottom:1px solid var(--border);gap:12px;transition:background .1s}
.contrib-row:last-child{border-bottom:none}
.contrib-row:hover{background:var(--surface2)}
.contrib-num{font-size:12px;color:var(--text3);font-family:'DM Mono',monospace;width:22px;flex-shrink:0;text-align:right}
.contrib-avatar{width:34px;height:34px;border-radius:50%;background:var(--primary-light);color:var(--primary);font-size:12px;font-weight:700;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.contrib-info{flex:1;min-width:0}
.contrib-name{font-size:13px;font-weight:700;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.contrib-role{font-size:10px;color:var(--text3);margin-top:1px}
.contrib-status{flex-shrink:0}

/* Toggle switch */
.toggle-wrap{display:flex;align-items:center;gap:8px}
.toggle{position:relative;width:42px;height:24px;flex-shrink:0}
.toggle input{opacity:0;width:0;height:0;position:absolute}
.toggle-slider{
  position:absolute;inset:0;border-radius:24px;
  background:var(--unpaid-bg);border:2px solid var(--border);
  cursor:pointer;transition:all .2s;
}
.toggle-slider::before{
  content:'';position:absolute;
  width:16px;height:16px;border-radius:50%;
  background:#aaa;top:2px;left:2px;
  transition:all .2s;
}
.toggle input:checked + .toggle-slider{background:var(--paid-bg);border-color:#7ddbbb}
.toggle input:checked + .toggle-slider::before{background:var(--paid);transform:translateX(18px)}
.toggle-label{font-size:12px;font-weight:600;color:var(--text3);min-width:46px}
.toggle input:checked ~ .toggle-label-text{color:var(--paid)}
.paid-label{font-size:12px;font-weight:700;color:var(--paid)}
.unpaid-label{font-size:12px;font-weight:600;color:var(--text3)}

/* Mobile contrib cards */
.contrib-cards{display:none;flex-direction:column;gap:10px}
@media(max-width:680px){
  .contrib-table-wrap{display:none}
  .contrib-cards{display:flex}
}
.contrib-card{background:var(--surface);border:1px solid var(--border);border-radius:12px;box-shadow:var(--shadow);display:flex;align-items:center;padding:14px 16px;gap:12px}
.contrib-card-info{flex:1;min-width:0}
.contrib-card-name{font-size:14px;font-weight:700;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.contrib-card-role{font-size:11px;color:var(--text3);margin-top:1px}
.contrib-card-toggle{flex-shrink:0;display:flex;flex-direction:column;align-items:center;gap:4px}

/* ── Modal ── */
.modal-overlay{display:none;position:fixed;inset:0;background:rgba(15,30,25,.45);backdrop-filter:blur(4px);z-index:1000;align-items:flex-end;justify-content:center}
.modal-overlay.open{display:flex}
.modal{background:var(--surface);border-radius:var(--rl) var(--rl) 0 0;box-shadow:var(--shadow-lg);width:100%;max-width:500px;max-height:92vh;overflow-y:auto;animation:sheetUp .22s ease}
@keyframes sheetUp{from{transform:translateY(30px);opacity:0}to{transform:translateY(0);opacity:1}}
.modal-header{padding:18px 20px 14px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;position:sticky;top:0;background:var(--surface);z-index:2}
.modal-header::before{content:'';position:absolute;top:8px;left:50%;transform:translateX(-50%);width:36px;height:4px;background:var(--border);border-radius:2px}
.modal-title{font-size:16px;font-weight:700;padding-top:4px}
.modal-close{width:28px;height:28px;border-radius:6px;background:var(--surface2);border:none;cursor:pointer;font-size:16px;display:flex;align-items:center;justify-content:center;color:var(--text2)}
.modal-close:hover{background:var(--border)}
.modal-body{padding:18px 20px}
.modal-footer{padding:14px 20px;border-top:1px solid var(--border);display:flex;gap:8px;justify-content:flex-end;position:sticky;bottom:0;background:var(--surface)}
.form-row{margin-bottom:14px}
.form-row label{display:block;font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.08em;color:var(--text3);margin-bottom:5px}
.form-row input,.form-row select,.form-row textarea{width:100%;padding:10px 12px;border:1.5px solid var(--border);border-radius:8px;font-family:'Plus Jakarta Sans',sans-serif;font-size:14px;color:var(--text);background:var(--surface);outline:none;transition:border-color .15s;-webkit-appearance:none}
.form-row input:focus,.form-row select:focus,.form-row textarea:focus{border-color:var(--primary)}
.form-row textarea{resize:vertical;min-height:70px}
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px}

/* Detail modal */
.detail-header{display:flex;align-items:center;gap:14px;margin-bottom:18px}
.detail-avatar{width:50px;height:50px;border-radius:14px;background:var(--primary-light);color:var(--primary);font-size:17px;font-weight:800;display:flex;align-items:center;justify-content:center}
.detail-name{font-size:17px;font-weight:800}
.detail-phone{font-size:12px;color:var(--text3);font-family:'DM Mono',monospace;margin-top:2px}
.detail-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:18px}
.detail-field{background:var(--surface2);border-radius:8px;padding:10px 12px}
.detail-field-label{font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.1em;color:var(--text3);margin-bottom:3px}
.detail-field-value{font-size:14px;font-weight:600;font-family:'DM Mono',monospace}
.payments-section-title{font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.1em;color:var(--text3);margin-bottom:10px}
.payment-box{border-radius:8px;padding:9px 6px;text-align:center;border:1.5px solid transparent}
.payment-box.paid{background:var(--paid-bg);border-color:#b2ddd1}
.payment-box.unpaid{background:var(--unpaid-bg);border-color:var(--border)}
.payment-box-month{font-size:9px;font-weight:700;text-transform:uppercase;letter-spacing:.07em;margin-bottom:3px}
.payment-box.paid .payment-box-month{color:var(--paid)}
.payment-box.unpaid .payment-box-month{color:var(--text3)}
.payment-box-amount{font-size:10px;font-family:'DM Mono',monospace;font-weight:500}
.payment-box.paid .payment-box-amount{color:var(--paid)}
.payment-box.unpaid .payment-box-amount{color:var(--text3)}

/* Toast */
.toast{position:fixed;bottom:calc(var(--bottom-nav-h) + 12px);left:50%;transform:translateX(-50%);background:var(--text);color:#fff;padding:11px 18px;border-radius:20px;font-size:13px;font-weight:500;box-shadow:var(--shadow-lg);z-index:9999;white-space:nowrap;animation:toastIn .2s ease}
@keyframes toastIn{from{opacity:0;transform:translateX(-50%) translateY(8px)}to{opacity:1;transform:translateX(-50%) translateY(0)}}

.confirm-text{font-size:14px;color:var(--text2);line-height:1.6}
.confirm-name{font-weight:700;color:var(--text)}
.empty-state{text-align:center;padding:40px 20px;color:var(--text3)}
.empty-state .icon{font-size:36px;margin-bottom:10px}

/* ── Responsive ── */
@media(max-width:960px){
  .stats-grid{grid-template-columns:repeat(2,1fr)}
  .dash-grid{grid-template-columns:1fr}
  .events-grid{grid-template-columns:1fr 1fr}
}
@media(max-width:680px){
  :root{--topbar-h:52px}
  .sidebar{transform:translateX(-100%)}
  .sidebar.open{transform:translateX(0)}
  .main{margin-left:0;padding-bottom:var(--bottom-nav-h)}
  .topbar{padding:0 14px}
  .topbar-title{font-size:14px}
  .topbar-sub{display:none}
  .hamburger{display:flex}
  .btn-add-desktop{display:none}
  .fab{display:flex}
  .bottom-nav{display:block}
  .content{padding:14px}
  .stats-grid{grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px}
  .stat-card{padding:14px}
  .stat-value{font-size:18px}
  .stat-sub{display:none}
  .dash-grid{grid-template-columns:1fr;gap:14px}
  .table-wrap{display:none}
  .member-cards{display:flex}
  .contrib-table-wrap{display:none}
  .contrib-cards{display:flex}
  .search-box{max-width:none}
  .modal{border-radius:20px 20px 0 0;max-height:96vh}
  .modal-footer .btn{flex:1;justify-content:center}
  .form-grid{grid-template-columns:1fr}
  .events-grid{grid-template-columns:1fr}
  .event-detail-stats{grid-template-columns:repeat(3,1fr)}
  .event-detail-hero-body{padding:16px}
  .event-detail-name{font-size:18px}
  .btn-export-label{display:none}
  .export-menu{right:auto;left:0}
}
@media print{
  .sidebar,.topbar-actions,.action-btns,.bottom-nav,.fab,.hamburger,.export-wrap{display:none!important}
  .main{margin-left:0}
  body{background:#fff}
}

/* ══════════════════════════════════════
   LOGIN SCREEN
══════════════════════════════════════ */
#login-screen{
  display:none;position:fixed;inset:0;z-index:2000;
  background:var(--primary);
  flex-direction:column;align-items:center;justify-content:center;
  padding:24px;
}
#login-screen.active{display:flex}

.login-box{
  background:#fff;border-radius:20px;
  width:100%;max-width:360px;
  overflow:hidden;
  box-shadow:0 20px 60px rgba(0,0,0,.25);
  animation:loginPop .3s cubic-bezier(.34,1.56,.64,1);
}
@keyframes loginPop{from{opacity:0;transform:translateY(24px) scale(.97)}to{opacity:1;transform:none}}

.login-hero{
  background:linear-gradient(135deg,var(--primary) 0%,var(--primary-mid) 100%);
  padding:32px 28px 24px;text-align:center;
}
.login-logo{font-size:36px;margin-bottom:10px}
.login-org{font-size:9px;letter-spacing:.22em;text-transform:uppercase;color:rgba(255,255,255,.6);margin-bottom:4px}
.login-title{font-size:22px;font-weight:800;color:#fff;line-height:1.1}
.login-sub{font-size:12px;color:rgba(255,255,255,.55);margin-top:4px}

.login-body{padding:28px}

/* Role selector tabs */
.role-tabs{display:flex;gap:8px;margin-bottom:24px;background:var(--surface2);border-radius:10px;padding:4px}
.role-tab{
  flex:1;padding:9px;border-radius:8px;border:none;cursor:pointer;
  font-family:'Plus Jakarta Sans',sans-serif;font-size:13px;font-weight:600;
  color:var(--text3);background:transparent;transition:all .15s;
  display:flex;align-items:center;justify-content:center;gap:6px;
}
.role-tab.active{background:#fff;color:var(--primary);box-shadow:0 1px 6px rgba(0,0,0,.1)}

.login-field{margin-bottom:16px}
.login-field label{display:block;font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.08em;color:var(--text3);margin-bottom:6px}
.login-field input{
  width:100%;padding:12px 14px;border:1.5px solid var(--border);border-radius:10px;
  font-family:'Plus Jakarta Sans',sans-serif;font-size:15px;color:var(--text);
  background:var(--surface);outline:none;transition:border-color .15s;
}
.login-field input:focus{border-color:var(--primary)}

.login-error{
  background:var(--danger-light);color:var(--danger);
  border:1px solid #f5c6c2;border-radius:8px;
  padding:10px 12px;font-size:13px;font-weight:500;
  margin-bottom:16px;display:none;
  animation:shake .3s ease;
}
.login-error.show{display:block}
@keyframes shake{0%,100%{transform:translateX(0)}25%{transform:translateX(-6px)}75%{transform:translateX(6px)}}

.login-btn{
  width:100%;padding:13px;border-radius:10px;border:none;
  background:var(--primary);color:#fff;
  font-family:'Plus Jakarta Sans',sans-serif;font-size:15px;font-weight:700;
  cursor:pointer;transition:background .15s;
}
.login-btn:hover{background:var(--primary-mid)}
.login-btn:active{transform:scale(.98)}

.login-footer{text-align:center;margin-top:16px;font-size:11px;color:var(--text3)}

/* Member-only read-only badge in topbar */
.member-badge{
  display:none;
  background:var(--primary-light);color:var(--primary);
  font-size:10px;font-weight:700;padding:3px 8px;border-radius:5px;
  text-transform:uppercase;letter-spacing:.07em;
}

/* Disable toggles in member view */
.member-mode .toggle input{pointer-events:none;opacity:.6}
.member-mode .toggle-slider{cursor:default}
.member-mode .contrib-row:hover{background:transparent}
.member-mode .contrib-card:hover{box-shadow:var(--shadow)}
</style>
</head>
<body>

<!-- ══════════════════════════════════
     LOGIN SCREEN
══════════════════════════════════ -->
<div id="login-screen" class="active">
  <div class="login-box">
    <div class="login-hero">
      <div class="login-logo">🤝</div>
      <div class="login-org">Mkoba Family · TPB</div>
      <div class="login-title">UMOJA WVJ</div>
      <div class="login-sub">Group Manager</div>
    </div>
    <div class="login-body">
      <div class="login-field">
        <label>Email</label>
        <input type="email" id="login-email" placeholder="your@email.com" autocomplete="email"
          onkeydown="if(event.key==='Enter')document.getElementById('login-password').focus()">
      </div>
      <div class="login-field">
        <label>Password</label>
        <input type="password" id="login-password" placeholder="Enter your password" autocomplete="current-password"
          onkeydown="if(event.key==='Enter')doLogin()">
      </div>
      <div class="login-error" id="login-error">Incorrect email or password.</div>
      <button class="login-btn" id="login-btn" onclick="doLogin()">Sign In →</button>
      <div class="login-footer">© 2026 UMOJA WVJ GROUP</div>
    </div>
  </div>
</div>

<div class="app">

<!-- Sidebar -->
<aside class="sidebar" id="sidebar">
  <div class="sidebar-logo">
    <div class="org-tag">Mkoba Family · TPB</div>
    <h1>UMOJA WVJ</h1>
    <div class="group-type">Group Manager v3.0</div>
  </div>
  <nav>
    <div class="nav-item active" onclick="showView('dashboard',this);closeSidebar()"><span class="icon">📊</span>Dashboard</div>
    <div class="nav-item" onclick="showView('members',this);closeSidebar()"><span class="icon">👥</span>Members</div>
    <div class="nav-item" onclick="showView('events',this);closeSidebar()"><span class="icon">📅</span>Events</div>
  </nav>
  <div class="sidebar-footer">
    <div style="margin-bottom:8px;color:rgba(255,255,255,.5)" id="sidebar-role-label">© 2026 UMOJA WVJ</div>
    <div style="cursor:pointer;color:rgba(255,255,255,.4);font-size:10px" onclick="doLogout()">⎋ Logout</div>
  </div>
</aside>
<div class="sidebar-overlay" id="sidebar-overlay" onclick="closeSidebar()"></div>

<!-- Main -->
<div class="main">
  <div class="topbar">
    <div class="topbar-left">
      <button class="hamburger" onclick="toggleSidebar()">
        <svg width="20" height="20" viewBox="0 0 20 20" fill="none">
          <rect y="3" width="20" height="2" rx="1" fill="currentColor"/>
          <rect y="9" width="20" height="2" rx="1" fill="currentColor"/>
          <rect y="15" width="20" height="2" rx="1" fill="currentColor"/>
        </svg>
      </button>
      <div>
        <div class="topbar-title" id="topbar-title">Dashboard</div>
        <div class="topbar-sub" id="topbar-sub">Overview &amp; summary</div>
      </div>
    </div>
    <div class="topbar-actions">
      <span class="member-badge" id="member-badge">👁 View Only</span>
      <div class="export-wrap" id="export-wrap-btn">
        <button class="btn btn-export btn-sm" onclick="toggleExportMenu()">⬇ <span class="btn-export-label">Export</span> ▾</button>
        <div class="export-menu" id="export-menu">
          <div class="export-item" onclick="exportCSV()">📄 Export CSV</div>
          <div class="export-item" onclick="exportPrint()">🖨 Print / PDF</div>
        </div>
      </div>
      <button class="btn btn-primary btn-sm btn-add-desktop" id="topbar-add-btn" onclick="handleTopbarAdd()">＋ Add Member</button>
      <button class="btn btn-ghost btn-sm" onclick="doLogout()" title="Logout">⎋ Logout</button>
    </div>
  </div>

  <div class="content">

    <!-- ══ DASHBOARD ══ -->
    <div class="view active" id="view-dashboard">
      <div class="stats-grid" id="stats-grid"></div>
      <div class="dash-grid">
        <div class="card">
          <div class="card-header">
            <span class="card-title">Member Payments</span>
            <button class="btn btn-ghost btn-sm" onclick="showView('members',document.querySelectorAll('.nav-item')[1])">All →</button>
          </div>
          <ul class="payment-list" id="dash-payment-list"></ul>
        </div>
        <div style="display:flex;flex-direction:column;gap:14px">
          <div class="card">
            <div class="card-header"><span class="card-title">Monthly Progress</span></div>
            <div class="month-progress" id="month-progress"></div>
          </div>
          <div class="card">
            <div class="card-header"><span class="card-title">Recent Events</span></div>
            <ul class="payment-list" id="dash-events-list"></ul>
          </div>
        </div>
      </div>
    </div>

    <!-- ══ MEMBERS ══ -->
    <div class="view" id="view-members">
      <div class="table-controls">
        <div class="search-box">
          <span>🔍</span>
          <input type="text" id="search-input" placeholder="Search members…" oninput="renderMembers()">
        </div>
        <select class="filter-sel" id="role-filter" onchange="renderMembers()">
          <option value="">All Roles</option>
          <option value="CHAIRPERSON">Chair</option>
          <option value="TREASURER">Treasurer</option>
          <option value="MEMBER">Member</option>
        </select>
      </div>
      <!-- Desktop table -->
      <div class="table-wrap">
        <div class="table-scroll">
          <table>
            <thead><tr>
              <th class="sticky-col" style="width:36px">#</th>
              <th class="sticky-col" style="left:36px;min-width:170px">Member</th>
              <th class="center">Role</th>
              <th class="right">Total Dep.</th>
              <th class="center">Mar</th>
              <th class="center">Apr</th><th class="center">May</th><th class="center">Jun</th>
              <th class="center">Jul</th><th class="center">Aug</th><th class="center">Sep</th>
              <th class="center">Oct</th><th class="center">Nov</th><th class="center">Dec</th>
              ${isAdmin()?'<th class="center">Actions</th>':''}
            </tr></thead>
            <tbody id="members-tbody"></tbody>
            <tfoot id="members-tfoot"></tfoot>
          </table>
        </div>
        <div id="empty-members" class="empty-state" style="display:none"><div class="icon">🔍</div><p>No members found</p></div>
      </div>
      <!-- Mobile cards -->
      <div class="member-cards" id="member-cards"></div>
      <div id="empty-cards" class="empty-state" style="display:none"><div class="icon">🔍</div><p>No members found</p></div>
    </div>

    <!-- ══ EVENTS ══ -->
    <div class="view" id="view-events">
      <!-- Event list screen -->
      <div id="events-list-screen">
        <div class="events-header">
          <div class="events-header-left">
            <h2>Events</h2>
            <p id="events-count-label">0 events created</p>
          </div>
          <button class="btn btn-primary btn-add-desktop" onclick="openAddEvent()">＋ New Event</button>
        </div>
        <div id="events-grid-wrap"></div>
      </div>
      <!-- Event detail screen -->
      <div id="events-detail-screen" style="display:none">
        <div class="back-btn" onclick="backToEvents()">← Back to Events</div>
        <div id="event-detail-content"></div>
      </div>
    </div>

  </div><!-- /content -->
</div><!-- /main -->

<!-- FAB -->
<button class="fab" id="main-fab" onclick="handleFab()" aria-label="Add">＋</button>

<!-- Bottom nav -->
<nav class="bottom-nav">
  <div class="bottom-nav-inner">
    <button class="bnav-item active" id="bnav-dashboard" onclick="showView('dashboard',null);setBnav('dashboard')">
      <span class="bnav-icon">📊</span>Dashboard
    </button>
    <button class="bnav-item" id="bnav-members" onclick="showView('members',null);setBnav('members')">
      <span class="bnav-icon">👥</span>Members
    </button>
    <button class="bnav-item" id="bnav-events" onclick="showView('events',null);setBnav('events')">
      <span class="bnav-icon">📅</span>Events
    </button>
  </div>
</nav>
</div><!-- /app -->

<!-- ══ ADD/EDIT MEMBER MODAL ══ -->
<div class="modal-overlay" id="modal-member">
  <div class="modal">
    <div class="modal-header">
      <span class="modal-title" id="modal-member-title">Add Member</span>
      <button class="modal-close" onclick="closeModal('modal-member')">✕</button>
    </div>
    <div class="modal-body">
      <input type="hidden" id="edit-id">
      <div class="form-grid">
        <div class="form-row"><label>Full Name</label><input type="text" id="f-name" placeholder="JOHN DOE" autocomplete="off"></div>
        <div class="form-row"><label>Phone</label><input type="tel" id="f-phone" placeholder="255XXXXXXXXX"></div>
      </div>
      <div class="form-grid">
        <div class="form-row">
          <label>Role</label>
          <select id="f-role"><option value="MEMBER">Member</option><option value="CHAIRPERSON">Chairperson</option><option value="TREASURER">Treasurer</option></select>
        </div>
        <div class="form-row"><label>Total Deposit (TZS)</label><input type="number" id="f-deposit" placeholder="0" min="0" step="1000" inputmode="numeric"></div>
      </div>
      <div class="form-row"><label>Type</label><input type="text" id="f-type" value="Mkoba Family"></div>
    </div>
    <div class="modal-footer">
      <button class="btn btn-ghost" onclick="closeModal('modal-member')">Cancel</button>
      <button class="btn btn-primary" onclick="saveMember()">Save</button>
    </div>
  </div>
</div>

<!-- ══ MEMBER DETAIL MODAL ══ -->
<div class="modal-overlay" id="modal-detail">
  <div class="modal" style="max-width:540px">
    <div class="modal-header">
      <span class="modal-title">Member Details</span>
      <button class="modal-close" onclick="closeModal('modal-detail')">✕</button>
    </div>
    <div class="modal-body" id="detail-body"></div>
    <div class="modal-footer">
      <button class="btn btn-ghost" onclick="closeModal('modal-detail')">Close</button>
      <button class="btn btn-primary" id="detail-edit-btn">✏️ Edit</button>
    </div>
  </div>
</div>

<!-- ══ PAYMENT MODAL ══ -->
<div class="modal-overlay" id="modal-payment">
  <div class="modal" style="max-width:520px">
    <div class="modal-header">
      <span class="modal-title" id="payment-modal-title">Record Payment</span>
      <button class="modal-close" onclick="closeModal('modal-payment')">✕</button>
    </div>
    <div class="modal-body">
      <p style="font-size:13px;color:var(--text2);margin-bottom:14px">Each period = <strong>TZS 10,000</strong>. Deposit auto-splits: March → April → … → December.</p>
      <input type="hidden" id="pay-member-id">
      <div class="form-row"><label>Total Deposit (TZS)</label><input type="number" id="pay-total" placeholder="0" min="0" step="1000" inputmode="numeric" oninput="previewSplit()"></div>
      <div id="split-preview"></div>
    </div>
    <div class="modal-footer">
      <button class="btn btn-ghost" onclick="closeModal('modal-payment')">Cancel</button>
      <button class="btn btn-primary" onclick="savePayment()">Save</button>
    </div>
  </div>
</div>

<!-- ══ ADD/EDIT EVENT MODAL ══ -->
<div class="modal-overlay" id="modal-event">
  <div class="modal" style="max-width:500px">
    <div class="modal-header">
      <span class="modal-title" id="modal-event-title">New Event</span>
      <button class="modal-close" onclick="closeModal('modal-event')">✕</button>
    </div>
    <div class="modal-body">
      <input type="hidden" id="ev-edit-id">
      <div class="form-row"><label>Event Name</label><input type="text" id="ev-name" placeholder="e.g. Monthly Contribution — March"></div>
      <div class="form-grid">
        <div class="form-row"><label>Date</label><input type="date" id="ev-date"></div>
        <div class="form-row"><label>Amount per Member (TZS)</label><input type="number" id="ev-amount" placeholder="10000" min="0" step="1000" inputmode="numeric"></div>
      </div>
      <div class="form-row"><label>Description / Notes</label><textarea id="ev-desc" placeholder="Optional notes about this event…"></textarea></div>
    </div>
    <div class="modal-footer">
      <button class="btn btn-ghost" onclick="closeModal('modal-event')">Cancel</button>
      <button class="btn btn-primary" onclick="saveEvent()">Save Event</button>
    </div>
  </div>
</div>

<!-- ══ CONFIRM DELETE MODAL ══ -->
<div class="modal-overlay" id="modal-confirm">
  <div class="modal" style="max-width:360px">
    <div class="modal-header">
      <span class="modal-title" id="confirm-title">Confirm Delete</span>
      <button class="modal-close" onclick="closeModal('modal-confirm')">✕</button>
    </div>
    <div class="modal-body">
      <p class="confirm-text" id="confirm-text">Are you sure?</p>
    </div>
    <div class="modal-footer">
      <button class="btn btn-ghost" onclick="closeModal('modal-confirm')">Cancel</button>
      <button class="btn btn-danger" id="confirm-ok-btn">Delete</button>
    </div>
  </div>
</div>

<script type="module">
/* ══════════════════════════════════════════════════════
   SUPABASE — official SDK via CDN for real Auth
══════════════════════════════════════════════════════ */
import { createClient } from 'https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2/+esm';

const SUPA_URL = 'https://fgofqrvvefmvqndnqmur.supabase.co';
const SUPA_KEY = 'sb_publishable_Q6gvDK7nthMDSw4VP5qOdQ_Kec2Weh3';
const supabase = createClient(SUPA_URL, SUPA_KEY);

/* ══════════════════════════════════════════════════════
   XSS PROTECTION — escape all user content before innerHTML
══════════════════════════════════════════════════════ */
function esc(str){
  if(str==null)return'';
  return String(str)
    .replace(/&/g,'&amp;').replace(/</g,'&lt;')
    .replace(/>/g,'&gt;').replace(/"/g,'&quot;').replace(/'/g,'&#39;');
}

/* ══════════════════════════════════════════════════════
   INACTIVITY AUTO-LOGOUT — 30 minutes
══════════════════════════════════════════════════════ */
let _inactivityTimer;
const INACTIVITY_MS = 30 * 60 * 1000;

function resetInactivityTimer(){
  clearTimeout(_inactivityTimer);
  _inactivityTimer = setTimeout(async()=>{
    toast('⏱ Session expired — logging out');
    setTimeout(doLogout, 1500);
  }, INACTIVITY_MS);
}
function startInactivityWatcher(){
  ['mousemove','keydown','touchstart','click','scroll'].forEach(ev=>
    document.addEventListener(ev, resetInactivityTimer, {passive:true}));
  resetInactivityTimer();
}
function stopInactivityWatcher(){
  clearTimeout(_inactivityTimer);
  ['mousemove','keydown','touchstart','click','scroll'].forEach(ev=>
    document.removeEventListener(ev, resetInactivityTimer));
}

/* ══════════════════════════════════════════════════════
   AUTH STATE — role comes from server, never client
══════════════════════════════════════════════════════ */
let _currentUser = null;
let _currentRole = null;
function isAdmin()  { return _currentRole === 'admin';  }
function isMember() { return _currentRole === 'member'; }

/* ══════════════════════════════════════════════════════
   LOGIN / LOGOUT
══════════════════════════════════════════════════════ */
async function doLogin(){
  const email    = document.getElementById('login-email').value.trim().toLowerCase();
  const password = document.getElementById('login-password').value;
  const errEl    = document.getElementById('login-error');
  const btn      = document.getElementById('login-btn');
  errEl.classList.remove('show');

  if(!email||!password){
    errEl.textContent='Please enter your email and password.';
    errEl.classList.add('show'); return;
  }

  btn.textContent='Signing in…'; btn.disabled=true;
  const { data, error } = await supabase.auth.signInWithPassword({ email, password });
  btn.textContent='Sign In →'; btn.disabled=false;

  if(error){
    errEl.textContent='Incorrect email or password.';
    errEl.classList.add('show');
    document.getElementById('login-password').value='';
    document.getElementById('login-password').focus();
    return;
  }

  const role = data.user?.user_metadata?.role;
  if(role!=='admin'&&role!=='member'){
    errEl.textContent='Account not authorised. Contact your admin.';
    errEl.classList.add('show');
    await supabase.auth.signOut(); return;
  }

  _currentUser=data.user; _currentRole=role;
  document.getElementById('login-screen').classList.remove('active');
  document.getElementById('login-email').value='';
  document.getElementById('login-password').value='';
  applyRoleUI(role);
  startInactivityWatcher();
  await fetchAll();
  renderDashboard();
}

async function doLogout(){
  stopInactivityWatcher();
  await supabase.auth.signOut();
  _currentUser=null; _currentRole=null;
  _members=[]; _events=[]; _contribs=[];
  document.getElementById('login-screen').classList.add('active');
  document.getElementById('login-error').classList.remove('show');
  setTimeout(()=>document.getElementById('login-email')?.focus(),200);
}

function applyRoleUI(role){
  const admin=role==='admin';
  document.getElementById('topbar-add-btn').style.display  =admin?'':'none';
  document.getElementById('export-wrap-btn').style.display =admin?'':'none';
  document.getElementById('member-badge').style.display    =admin?'none':'inline-flex';
  document.getElementById('main-fab').style.display        =admin?'':'none';
  document.getElementById('sidebar-role-label').textContent=
    admin?'🔐 Admin · UMOJA WVJ':'👁 Member View · UMOJA WVJ';
  document.body.classList.toggle('member-mode',!admin);
}

/* ══════════════════════════════════════════════════════
   DATABASE HELPERS — Supabase SDK (no raw fetch)
══════════════════════════════════════════════════════ */
async function dbGet(table,opts={}){
  let q=supabase.from(table).select(opts.select||'*');
  if(opts.order) q=q.order(opts.order,{ascending:opts.asc??true});
  const{data,error}=await q;
  if(error)throw error;
  return data||[];
}
async function dbInsert(table,body){
  const{data,error}=await supabase.from(table).insert(body).select();
  if(error)throw error;
  return data;
}
async function dbUpdate(table,match,body){
  let q=supabase.from(table).update(body);
  Object.entries(match).forEach(([k,v])=>{q=q.eq(k,v);});
  const{data,error}=await q.select();
  if(error)throw error;
  return data;
}
async function dbDelete(table,match){
  let q=supabase.from(table).delete();
  Object.entries(match).forEach(([k,v])=>{q=q.eq(k,v);});
  const{error}=await q;
  if(error)throw error;
}
async function dbUpsert(table,body,onConflict){
  const{data,error}=await supabase.from(table).upsert(body,{onConflict}).select();
  if(error)throw error;
  return data;
}

/* ══════════════════════════════════════════════════════
   CACHE
══════════════════════════════════════════════════════ */
let _members=[],_events=[],_contribs=[];

async function fetchAll(){
  showLoader(true);
  try{
    const[members,events,contribs]=await Promise.all([
      dbGet('members',{order:'deposit',asc:false}),
      dbGet('events',{order:'date',asc:false}),
      dbGet('contributions'),
    ]);
    _members=members;
    _events=events;
    _contribs=contribs.map(c=>({...c,member_id:Number(c.member_id)}));
    _events.forEach(ev=>{ev.contributions=_contribs.filter(c=>c.event_id===ev.id);});
  }catch(e){toast('❌ Failed to load data');console.error(e);}
  showLoader(false);
}

/* ══════════════════════════════════════════════════════
   LOADER
══════════════════════════════════════════════════════ */
function showLoader(on){
  let el=document.getElementById('global-loader');
  if(!el){
    el=document.createElement('div');el.id='global-loader';
    el.style.cssText='position:fixed;inset:0;background:rgba(255,255,255,.75);display:flex;align-items:center;justify-content:center;z-index:9998;backdrop-filter:blur(2px);font-family:\'Plus Jakarta Sans\',sans-serif;font-size:14px;color:var(--primary);font-weight:600;gap:10px;';
    el.innerHTML='<span style="font-size:22px;animation:spin .8s linear infinite">⏳</span> Loading…';
    document.body.appendChild(el);
    const s=document.createElement('style');
    s.textContent='@keyframes spin{to{transform:rotate(360deg)}}';
    document.head.appendChild(s);
  }
  el.style.display=on?'flex':'none';
}

/* ══════════════════════════════════════════════════════
   CONFIG
══════════════════════════════════════════════════════ */
const MONTHS=['mar','apr','may','jun','jul','aug','sep','oct','nov','dec'];
const ML={mar:'March',apr:'April',may:'May',jun:'June',jul:'July',aug:'August',sep:'September',oct:'October',nov:'November',dec:'December'};
const PER=10000;

/* ══════════════════════════════════════════════════════
   HELPERS
══════════════════════════════════════════════════════ */
function splitDep(dep){
  const r={};MONTHS.forEach(m=>r[m]=0);
  let rem=Math.max(0,dep);
  for(const m of MONTHS){if(rem<=0)break;r[m]=Math.min(rem,PER);rem-=r[m];}
  return r;
}
function depStatus(a){return a<=0?'unpaid':a>=PER?'paid':'partial';}
function pill(a){
  const s=depStatus(a),l=s==='paid'?`${fmt(a)} ✓`:s==='partial'?`${fmt(a)}…`:'—';
  return`<span class="pay-pill pay-${s==='partial'?'unpaid':s}">${l}</span>`;
}
function ini(n){if(!n)return'?';return n.split(' ').slice(0,2).map(w=>w[0]).join('').toUpperCase();}
function fmt(n){return Number(n).toLocaleString();}
function fmtDate(d){
  if(!d)return'';
  try{const dt=new Date(d+'T00:00:00');return dt.toLocaleDateString('en-GB',{day:'2-digit',month:'short',year:'numeric'});}
  catch{return esc(d);}
}

/* ══════════════════════════════════════════════════════
   SIDEBAR
══════════════════════════════════════════════════════ */
function toggleSidebar(){document.getElementById('sidebar').classList.toggle('open');document.getElementById('sidebar-overlay').classList.toggle('open');}
function closeSidebar(){document.getElementById('sidebar').classList.remove('open');document.getElementById('sidebar-overlay').classList.remove('open');}

/* ══════════════════════════════════════════════════════
   NAV
══════════════════════════════════════════════════════ */
function setBnav(id){
  document.querySelectorAll('.bnav-item').forEach(b=>b.classList.remove('active'));
  const el=document.getElementById('bnav-'+id);if(el)el.classList.add('active');
}
let _currentView='dashboard';
function handleTopbarAdd(){if(_currentView==='events')openAddEvent();else openAddMember();}
function handleFab(){if(_currentView==='events')openAddEvent();else openAddMember();}
function updateTopbarAddBtn(view){
  const btn=document.getElementById('topbar-add-btn');
  if(btn)btn.textContent=view==='events'?'＋ New Event':'＋ Add Member';
}

/* ══════════════════════════════════════════════════════
   VIEWS
══════════════════════════════════════════════════════ */
const VMETA={
  dashboard:['Dashboard','Overview & summary'],
  members:  ['Members','All group members'],
  events:   ['Events','Group events & contributions']
};
async function showView(id,navEl){
  document.querySelectorAll('.view').forEach(v=>v.classList.remove('active'));
  document.querySelectorAll('.nav-item').forEach(n=>n.classList.remove('active'));
  document.getElementById('view-'+id).classList.add('active');
  if(navEl)navEl.classList.add('active');
  const[t,s]=VMETA[id];
  document.getElementById('topbar-title').textContent=t;
  document.getElementById('topbar-sub').textContent=s;
  _currentView=id; updateTopbarAddBtn(id); setBnav(id);
  await fetchAll();
  if(id==='dashboard')renderDashboard();
  if(id==='members')  renderMembers();
  if(id==='events')   renderEventsList();
}

/* ══════════════════════════════════════════════════════
   DASHBOARD
══════════════════════════════════════════════════════ */
function renderDashboard(){
  const M=_members,E=_events;
  const total=M.reduce((s,m)=>s+m.deposit,0);
  const paid=M.filter(m=>m.deposit>=PER).length;
  const unpaid=M.filter(m=>m.deposit===0).length;
  document.getElementById('stats-grid').innerHTML=`
    <div class="stat-card green"><div class="stat-icon">💰</div><div class="stat-value">${fmt(total)}</div><div class="stat-label">Collected (TZS)</div><div class="stat-sub">${M.length} members</div></div>
    <div class="stat-card amber"><div class="stat-icon">✅</div><div class="stat-value">${paid}</div><div class="stat-label">March Paid</div><div class="stat-sub">of ${M.length}</div></div>
    <div class="stat-card blue"><div class="stat-icon">📅</div><div class="stat-value">${E.length}</div><div class="stat-label">Events</div><div class="stat-sub">total created</div></div>
    <div class="stat-card red"><div class="stat-icon">❌</div><div class="stat-value">${unpaid}</div><div class="stat-label">Not Paid</div><div class="stat-sub">zero deposit</div></div>`;
  document.getElementById('dash-payment-list').innerHTML=
    [...M].sort((a,b)=>b.deposit-a.deposit).map(m=>`
      <li class="payment-item">
        <div class="member-avatar">${ini(m.name)}</div>
        <span class="payment-name">${esc(m.name)}</span>
        <span class="payment-deposit">TZS ${fmt(m.deposit)}</span>
        <span class="status-dot dot-${depStatus(m.deposit)}"></span>
      </li>`).join('');
  const maxE=M.length*PER;
  document.getElementById('month-progress').innerHTML=MONTHS.map(mo=>{
    const a=M.reduce((s,m)=>s+splitDep(m.deposit)[mo],0);
    const p=maxE>0?Math.round(a/maxE*100):0;
    return`<div class="month-row">
      <span class="month-label">${ML[mo].slice(0,3)}</span>
      <div class="progress-bar"><div class="progress-fill ${p>=100?'':p>0?'partial':''}" style="width:${p}%"></div></div>
      <span class="month-pct">${p}%</span>
    </div>`;}).join('');
  const evEl=document.getElementById('dash-events-list');
  if(!E.length){
    evEl.innerHTML='<li class="payment-item" style="color:var(--text3);font-size:13px;justify-content:center">No events yet</li>';
  } else {
    evEl.innerHTML=[...E].slice(0,4).map(ev=>{
      const paidCount=(ev.contributions||[]).filter(c=>c.paid).length;
      return`<li class="payment-item" style="cursor:pointer" onclick="openEventDetail('${esc(ev.id)}')">
        <div class="member-avatar" style="background:#fef3e2;color:var(--accent);font-size:16px">📅</div>
        <div style="flex:1;min-width:0"><div class="payment-name">${esc(ev.name)}</div><div style="font-size:10px;color:var(--text3);font-family:'DM Mono',monospace">${fmtDate(ev.date)}</div></div>
        <span style="font-size:11px;font-family:'DM Mono',monospace;color:var(--text2)">${paidCount}/${M.length}</span>
      </li>`;}).join('');
  }
}

/* ══════════════════════════════════════════════════════
   MEMBERS
══════════════════════════════════════════════════════ */
function renderMembers(){
  const q=(document.getElementById('search-input')?.value||'').toLowerCase();
  const rf=document.getElementById('role-filter')?.value||'';
  const list=_members.filter(m=>(!q||(m.name.toLowerCase().includes(q)||m.phone.includes(q)))&&(!rf||m.role===rf));
  const tbody=document.getElementById('members-tbody');
  const empty=document.getElementById('empty-members');
  if(!list.length){
    tbody.innerHTML='';empty.style.display='block';
    document.getElementById('members-tfoot').innerHTML='';
  } else {
    empty.style.display='none';
    tbody.innerHTML=list.map((m,i)=>{
      const sp=splitDep(m.deposit);
      const rc=m.role==='CHAIRPERSON'?'role-chair':m.role==='TREASURER'?'role-treasurer':'role-member';
      return`<tr onclick="viewMemberDetail(${m.id})">
        <td class="sticky-col" style="color:var(--text3);font-size:12px;font-family:'DM Mono',monospace">${i+1}</td>
        <td class="sticky-col" style="left:36px">
          <div class="member-name-cell">
            <div class="member-avatar">${ini(m.name)}</div>
            <div><div class="member-name">${esc(m.name)}</div><div class="member-phone">${esc(m.phone)}</div></div>
          </div>
        </td>
        <td class="center"><span class="role-pill ${rc}">${esc(m.role)}</span></td>
        <td class="right"><span class="${m.deposit>0?'amount-cell':'amount-zero'}">${fmt(m.deposit)}</span></td>
        ${MONTHS.map(mo=>`<td class="center">${pill(sp[mo])}</td>`).join('')}
        <td class="center" onclick="event.stopPropagation()" ${!isAdmin()?'style="display:none"':''}>
          <div class="action-btns">
            <button class="btn btn-ghost btn-sm btn-icon" onclick="openEditMember(${m.id})">✏️</button>
            <button class="btn btn-ghost btn-sm btn-icon" onclick="openPayment(${m.id})">💳</button>
            <button class="btn btn-danger btn-sm btn-icon" onclick="askDeleteMember(${m.id})">🗑</button>
          </div>
        </td>
      </tr>`;}).join('');
    const tots={};
    MONTHS.forEach(mo=>tots[mo]=list.reduce((s,m)=>s+splitDep(m.deposit)[mo],0));
    const grand=list.reduce((s,m)=>s+m.deposit,0);
    document.getElementById('members-tfoot').innerHTML=`<tr>
      <td class="sticky-col"></td>
      <td class="sticky-col label-cell" style="left:36px">TOTALS (${list.length})</td>
      <td></td><td class="right">${fmt(grand)}</td>
      ${MONTHS.map(mo=>`<td class="center">${tots[mo]>0?fmt(tots[mo]):''}</td>`).join('')}
      <td></td></tr>`;
  }
  const cardsEl=document.getElementById('member-cards');
  const emptyC=document.getElementById('empty-cards');
  if(!list.length){cardsEl.innerHTML='';emptyC.style.display='block';}
  else{
    emptyC.style.display='none';
    cardsEl.innerHTML=list.map(m=>{
      const sp=splitDep(m.deposit);
      const rc=m.role==='CHAIRPERSON'?'role-chair':m.role==='TREASURER'?'role-treasurer':'role-member';
      const pp=MONTHS.slice(0,4).map(mo=>{const a=sp[mo],s=depStatus(a);return`<span class="pay-pill pay-${s==='partial'?'unpaid':s}" style="font-size:9px">${ML[mo].slice(0,3)}:${a>0?fmt(a):'—'}</span>`;}).join('');
      return`<div class="member-card" onclick="viewMemberDetail(${m.id})">
        <div class="member-card-top">
          <div class="mc-avatar">${ini(m.name)}</div>
          <div class="mc-info"><div class="mc-name">${esc(m.name)}</div><div class="mc-phone">${esc(m.phone)}</div></div>
          <div class="mc-deposit"><div class="mc-dep-val ${m.deposit===0?'zero':''}">${fmt(m.deposit)}</div><div class="mc-dep-label">TZS</div></div>
        </div>
        <div class="member-card-pills" onclick="event.stopPropagation()">
          <span class="role-pill ${rc} mc-role">${esc(m.role)}</span>${pp}
        </div>
        <div class="member-card-actions" onclick="event.stopPropagation()" ${!isAdmin()?'style="display:none"':''}>
          <button class="btn btn-ghost btn-sm" onclick="openEditMember(${m.id})">✏️ Edit</button>
          <button class="btn btn-ghost btn-sm" onclick="openPayment(${m.id})">💳 Pay</button>
          <button class="btn btn-danger btn-sm" onclick="askDeleteMember(${m.id})">🗑</button>
        </div>
      </div>`;}).join('');
  }
}

/* ══════════════════════════════════════════════════════
   EVENTS LIST
══════════════════════════════════════════════════════ */
function renderEventsList(){
  const events=_events,members=_members;
  document.getElementById('events-count-label').textContent=`${events.length} event${events.length!==1?'s':''} created`;
  const addEvBtn=document.querySelector('#events-list-screen .btn-add-desktop');
  if(addEvBtn)addEvBtn.style.display=isAdmin()?'':'none';
  const wrap=document.getElementById('events-grid-wrap');
  if(!events.length){
    wrap.innerHTML=`<div class="events-empty"><div class="icon">📅</div><h3>No events yet</h3><p>Create your first event to start tracking member contributions.</p></div>`;return;
  }
  wrap.innerHTML=`<div class="events-grid">${events.map(ev=>{
    const contribs=ev.contributions||[];
    const paidCount=contribs.filter(c=>c.paid).length;
    const total=members.length,pct=total>0?Math.round(paidCount/total*100):0;
    const collected=paidCount*(ev.amount||0);
    return`<div class="event-card" onclick="openEventDetail('${esc(ev.id)}')">
      <div class="event-card-banner"></div>
      <div class="event-card-body">
        <div class="event-card-top">
          <div class="event-name">${esc(ev.name)}</div>
          <span class="event-date-badge">📅 ${fmtDate(ev.date)}</span>
        </div>
        <div class="event-desc">${ev.description?esc(ev.description):'<span style="color:var(--border)">No description</span>'}</div>
        <div class="event-amount-row">
          <span class="event-amount-label">Per member</span>
          <span class="event-amount-val">TZS ${fmt(ev.amount||0)}</span>
        </div>
        <div class="event-progress-row">
          <div class="event-prog-bar-wrap"><div class="event-prog-bar"><div class="event-prog-fill" style="width:${pct}%"></div></div></div>
          <span class="event-prog-label">${pct}% paid</span>
        </div>
        <div class="event-counters">
          <div class="ev-counter paid"><div class="ev-counter-val">${paidCount}</div><div class="ev-counter-label">Paid</div></div>
          <div class="ev-counter unpaid"><div class="ev-counter-val">${total-paidCount}</div><div class="ev-counter-label">Pending</div></div>
          <div class="ev-counter total"><div class="ev-counter-val">TZS ${fmt(collected)}</div><div class="ev-counter-label">Collected</div></div>
        </div>
      </div>
      <div class="event-card-footer" onclick="event.stopPropagation()">
        ${isAdmin()?`<button class="btn btn-ghost btn-sm" onclick="openEditEvent('${esc(ev.id)}')">✏️ Edit</button>
        <button class="btn btn-danger btn-sm" onclick="askDeleteEvent('${esc(ev.id)}')">🗑 Delete</button>`:''}
        <button class="btn btn-primary btn-sm" style="margin-left:auto" onclick="openEventDetail('${esc(ev.id)}')">View →</button>
      </div>
    </div>`;}).join('')}</div>`;
}

/* ══════════════════════════════════════════════════════
   EVENT DETAIL
══════════════════════════════════════════════════════ */
async function openEventDetail(evId){
  document.getElementById('events-list-screen').style.display='none';
  document.getElementById('events-detail-screen').style.display='block';
  await fetchAll();renderEventDetail(evId);
}
function renderEventDetail(evId){
  const ev=_events.find(e=>e.id===evId);if(!ev)return;
  const members=_members;
  const contribs=_contribs.filter(c=>c.event_id===evId);
  const paidCount=contribs.filter(c=>c.paid).length;
  const total=members.length,pct=total>0?Math.round(paidCount/total*100):0;
  const collected=paidCount*(ev.amount||0),outstanding=(total-paidCount)*(ev.amount||0);
  const sorted=[...members].sort((a,b)=>{
    const aP=contribs.find(c=>c.member_id===a.id)?.paid||false;
    const bP=contribs.find(c=>c.member_id===b.id)?.paid||false;
    if(aP===bP)return a.name.localeCompare(b.name);
    return aP?1:-1;
  });
  const safeId=esc(evId);
  document.getElementById('event-detail-content').innerHTML=`
    <div class="event-detail-hero">
      <div class="event-detail-hero-banner"></div>
      <div class="event-detail-hero-body">
        <div class="event-detail-top">
          <div>
            <div class="event-detail-name">${esc(ev.name)}</div>
            <div class="event-detail-meta">
              <span class="meta-badge meta-date">📅 ${fmtDate(ev.date)}</span>
              <span class="meta-badge meta-amount">TZS ${fmt(ev.amount||0)} / member</span>
            </div>
          </div>
          <div style="display:flex;gap:6px;flex-shrink:0">
            ${isAdmin()?`<button class="btn btn-ghost btn-sm" onclick="openEditEvent('${safeId}')">✏️ Edit</button>
            <button class="btn btn-danger btn-sm" onclick="askDeleteEvent('${safeId}')">🗑</button>`:''}
          </div>
        </div>
        ${ev.description?`<div class="event-detail-desc">${esc(ev.description)}</div>`:''}
        <div class="event-detail-stats">
          <div class="eds-card paid"><div class="eds-val" id="eds-paid-${safeId}">${paidCount}</div><div class="eds-label">Paid</div></div>
          <div class="eds-card unpaid"><div class="eds-val" id="eds-pend-${safeId}">${total-paidCount}</div><div class="eds-label">Pending</div></div>
          <div class="eds-card total"><div class="eds-val" id="eds-coll-${safeId}">TZS ${fmt(collected)}</div><div class="eds-label">Collected</div></div>
        </div>
        <div style="margin-top:14px">
          <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px">
            <span style="font-size:12px;font-weight:600;color:var(--text2)">Collection progress</span>
            <span style="font-size:12px;font-family:'DM Mono',monospace;color:var(--text3)" id="eds-prog-label-${safeId}">${pct}% · TZS ${fmt(outstanding)} outstanding</span>
          </div>
          <div style="height:8px;background:var(--surface2);border-radius:4px;overflow:hidden">
            <div id="eds-prog-bar-${safeId}" style="height:100%;width:${pct}%;background:var(--primary);border-radius:4px;transition:width .4s"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="contrib-section-title">Member Contributions (${total})</div>
    <div class="contrib-table-wrap">
      ${sorted.map((m,i)=>{
        const c=contribs.find(x=>x.member_id===m.id);
        const isPaid=c?.paid||false;
        const rc=m.role==='CHAIRPERSON'?'role-chair':m.role==='TREASURER'?'role-treasurer':'role-member';
        return`<div class="contrib-row">
          <span class="contrib-num">${i+1}</span>
          <div class="contrib-avatar">${ini(m.name)}</div>
          <div class="contrib-info">
            <div class="contrib-name">${esc(m.name)}</div>
            <div class="contrib-role"><span class="role-pill ${rc}">${esc(m.role)}</span></div>
          </div>
          <div class="contrib-status">
            <div class="toggle-wrap">
              <label class="toggle">
                <input type="checkbox" ${isPaid?'checked':''} ${!isAdmin()?'disabled':''} onchange="toggleContrib('${safeId}',${m.id},this.checked)">
                <span class="toggle-slider"></span>
              </label>
              <span class="${isPaid?'paid-label':'unpaid-label'}" id="tlabel-${safeId}-${m.id}">${isPaid?'✓ Paid':'Pending'}</span>
            </div>
          </div>
        </div>`;}).join('')}
    </div>
    <div class="contrib-cards">
      ${sorted.map(m=>{
        const c=contribs.find(x=>x.member_id===m.id);
        const isPaid=c?.paid||false;
        const rc=m.role==='CHAIRPERSON'?'role-chair':m.role==='TREASURER'?'role-treasurer':'role-member';
        return`<div class="contrib-card">
          <div class="contrib-avatar">${ini(m.name)}</div>
          <div class="contrib-card-info">
            <div class="contrib-card-name">${esc(m.name)}</div>
            <div class="contrib-card-role"><span class="role-pill ${rc}">${esc(m.role)}</span></div>
          </div>
          <div class="contrib-card-toggle">
            <label class="toggle">
              <input type="checkbox" ${isPaid?'checked':''} ${!isAdmin()?'disabled':''} onchange="toggleContrib('${safeId}',${m.id},this.checked)">
              <span class="toggle-slider"></span>
            </label>
            <span class="${isPaid?'paid-label':'unpaid-label'}" id="clabel-${safeId}-${m.id}" style="font-size:10px">${isPaid?'Paid':'Pending'}</span>
          </div>
        </div>`;}).join('')}
    </div>`;
}
function backToEvents(){
  document.getElementById('events-list-screen').style.display='';
  document.getElementById('events-detail-screen').style.display='none';
  renderEventsList();
}

/* ══════════════════════════════════════════════════════
   TOGGLE CONTRIBUTION
══════════════════════════════════════════════════════ */
async function toggleContrib(evId,memberId,paid){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  memberId=Number(memberId);
  const existing=_contribs.find(c=>c.event_id===evId&&c.member_id===memberId);
  const prevPaid=existing?.paid||false;
  const l1=document.getElementById(`tlabel-${evId}-${memberId}`);
  const l2=document.getElementById(`clabel-${evId}-${memberId}`);
  function setLabels(p){
    if(l1){l1.textContent=p?'✓ Paid':'Pending';l1.className=p?'paid-label':'unpaid-label';}
    if(l2){l2.textContent=p?'Paid':'Pending';l2.className=p?'paid-label':'unpaid-label';l2.style.fontSize='10px';}
  }
  setLabels(paid);
  try{
    await dbUpsert('contributions',{event_id:evId,member_id:memberId,paid,updated_at:new Date().toISOString()},'event_id,member_id');
    const idx=_contribs.findIndex(c=>c.event_id===evId&&c.member_id===memberId);
    if(idx!==-1)_contribs[idx].paid=paid;
    else _contribs.push({event_id:evId,member_id:memberId,paid});
    refreshEventHeroStats(evId);
    toast(paid?'✅ Marked as paid':'⏪ Marked as pending');
  }catch(e){
    setLabels(prevPaid);
    document.querySelectorAll('input[type="checkbox"]').forEach(cb=>{
      if(cb.getAttribute('onchange')?.includes(`'${evId}',${memberId}`))cb.checked=prevPaid;
    });
    toast('❌ Failed to save');console.error(e);
  }
}
function refreshEventHeroStats(evId){
  const contribs=_contribs.filter(c=>c.event_id===evId);
  const ev=_events.find(e=>e.id===evId);
  const total=_members.length;
  const paidCount=contribs.filter(c=>c.paid).length;
  const pct=total>0?Math.round(paidCount/total*100):0;
  const collected=paidCount*(ev?.amount||0);
  const outstanding=(total-paidCount)*(ev?.amount||0);
  const el=id=>document.getElementById(id);
  if(el(`eds-paid-${evId}`))    el(`eds-paid-${evId}`).textContent=paidCount;
  if(el(`eds-pend-${evId}`))    el(`eds-pend-${evId}`).textContent=total-paidCount;
  if(el(`eds-coll-${evId}`))    el(`eds-coll-${evId}`).textContent=`TZS ${fmt(collected)}`;
  if(el(`eds-prog-bar-${evId}`))el(`eds-prog-bar-${evId}`).style.width=pct+'%';
  if(el(`eds-prog-label-${evId}`))el(`eds-prog-label-${evId}`).textContent=`${pct}% · TZS ${fmt(outstanding)} outstanding`;
}

/* ══════════════════════════════════════════════════════
   ADD / EDIT EVENT
══════════════════════════════════════════════════════ */
function openAddEvent(){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  document.getElementById('modal-event-title').textContent='New Event';
  ['ev-edit-id','ev-name','ev-desc'].forEach(i=>document.getElementById(i).value='');
  document.getElementById('ev-date').value=new Date().toISOString().slice(0,10);
  document.getElementById('ev-amount').value='10000';
  openModal('modal-event');
}
function openEditEvent(evId){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const ev=_events.find(e=>e.id===evId);if(!ev)return;
  document.getElementById('modal-event-title').textContent='Edit Event';
  document.getElementById('ev-edit-id').value=evId;
  document.getElementById('ev-name').value=ev.name;
  document.getElementById('ev-date').value=ev.date;
  document.getElementById('ev-amount').value=ev.amount||10000;
  document.getElementById('ev-desc').value=ev.description||'';
  openModal('modal-event');
}
async function saveEvent(){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const name=document.getElementById('ev-name').value.trim();
  const date=document.getElementById('ev-date').value;
  const amount=parseInt(document.getElementById('ev-amount').value)||0;
  const description=document.getElementById('ev-desc').value.trim();
  const eid=document.getElementById('ev-edit-id').value;
  if(!name){toast('⚠️ Event name required');return;}
  if(!date){toast('⚠️ Date required');return;}
  showLoader(true);
  try{
    if(eid){
      await dbUpdate('events',{id:eid},{name,date,amount,description});
      toast('✅ Event updated');
    } else {
      const evId='ev_'+Date.now();
      await dbInsert('events',{id:evId,name,date,amount,description});
      if(_members.length) await dbInsert('contributions',_members.map(m=>({event_id:evId,member_id:m.id,paid:false})));
      toast('✅ Event created');
    }
    closeModal('modal-event');await fetchAll();renderEventsList();
  }catch(e){toast('❌ Failed to save event');console.error(e);}
  showLoader(false);
}

/* ══════════════════════════════════════════════════════
   DELETE EVENT
══════════════════════════════════════════════════════ */
function askDeleteEvent(evId){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const ev=_events.find(e=>e.id===evId);if(!ev)return;
  document.getElementById('confirm-title').textContent='Delete Event';
  document.getElementById('confirm-text').innerHTML=`Delete event <strong>"${esc(ev.name)}"</strong>? All contribution data will be lost.`;
  document.getElementById('confirm-ok-btn').textContent='🗑 Delete Event';
  document.getElementById('confirm-ok-btn').onclick=async()=>{
    showLoader(true);
    try{
      await dbDelete('events',{id:evId});
      toast('🗑 Event deleted');closeModal('modal-confirm');
      backToEvents();await fetchAll();renderEventsList();
    }catch(e){toast('❌ Failed to delete');console.error(e);}
    showLoader(false);
  };
  openModal('modal-confirm');
}

/* ══════════════════════════════════════════════════════
   MEMBER CRUD
══════════════════════════════════════════════════════ */
function openAddMember(){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  document.getElementById('modal-member-title').textContent='Add Member';
  ['edit-id','f-name','f-phone','f-deposit'].forEach(i=>document.getElementById(i).value='');
  document.getElementById('f-role').value='MEMBER';
  document.getElementById('f-type').value='Mkoba Family';
  openModal('modal-member');
}
function openEditMember(id){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const m=_members.find(x=>x.id===id);if(!m)return;
  document.getElementById('modal-member-title').textContent='Edit Member';
  document.getElementById('edit-id').value=id;
  document.getElementById('f-name').value=m.name;
  document.getElementById('f-phone').value=m.phone;
  document.getElementById('f-role').value=m.role;
  document.getElementById('f-deposit').value=m.deposit;
  document.getElementById('f-type').value=m.type;
  openModal('modal-member');
}
async function saveMember(){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const name=document.getElementById('f-name').value.trim().toUpperCase();
  const phone=document.getElementById('f-phone').value.trim();
  const role=document.getElementById('f-role').value;
  const deposit=parseInt(document.getElementById('f-deposit').value)||0;
  const type=document.getElementById('f-type').value.trim();
  const eid=document.getElementById('edit-id').value;
  if(!name||!phone){toast('⚠️ Name and phone required');return;}
  showLoader(true);
  try{
    if(eid){
      await dbUpdate('members',{id:parseInt(eid)},{name,phone,role,deposit,type});
      toast('✅ Member updated');
    } else {
      const[newMember]=await dbInsert('members',{name,phone,role,deposit,type});
      if(_events.length&&newMember?.id)
        await dbInsert('contributions',_events.map(ev=>({event_id:ev.id,member_id:newMember.id,paid:false})));
      toast('✅ Member added');
    }
    closeModal('modal-member');await fetchAll();renderMembers();renderDashboard();
  }catch(e){toast('❌ Failed to save member');console.error(e);}
  showLoader(false);
}
function askDeleteMember(id){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const m=_members.find(x=>x.id===id);if(!m)return;
  document.getElementById('confirm-title').textContent='Delete Member';
  document.getElementById('confirm-text').innerHTML=`Delete <strong>${esc(m.name)}</strong>? This cannot be undone.`;
  document.getElementById('confirm-ok-btn').textContent='🗑 Delete Member';
  document.getElementById('confirm-ok-btn').onclick=async()=>{
    showLoader(true);
    try{
      await dbDelete('members',{id});
      toast('🗑 Member deleted');closeModal('modal-confirm');
      await fetchAll();renderMembers();renderDashboard();
    }catch(e){toast('❌ Failed to delete');console.error(e);}
    showLoader(false);
  };
  openModal('modal-confirm');
}
function viewMemberDetail(id){
  const m=_members.find(x=>x.id===id);if(!m)return;
  const sp=splitDep(m.deposit);
  document.getElementById('detail-body').innerHTML=`
    <div class="detail-header">
      <div class="detail-avatar">${ini(m.name)}</div>
      <div><div class="detail-name">${esc(m.name)}</div><div class="detail-phone">${esc(m.phone)}</div></div>
    </div>
    <div class="detail-grid">
      <div class="detail-field"><div class="detail-field-label">Role</div><div class="detail-field-value">${esc(m.role)}</div></div>
      <div class="detail-field"><div class="detail-field-label">Type</div><div class="detail-field-value">${esc(m.type)}</div></div>
      <div class="detail-field"><div class="detail-field-label">Total Deposit</div><div class="detail-field-value" style="color:var(--primary)">TZS ${fmt(m.deposit)}</div></div>
      <div class="detail-field"><div class="detail-field-label">Periods Covered</div><div class="detail-field-value">${Math.floor(m.deposit/PER)} / ${MONTHS.length}</div></div>
    </div>
    <div class="payments-section-title">Period Breakdown</div>
    <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:7px">
      ${MONTHS.map(mo=>{const a=sp[mo],s=depStatus(a);return`<div class="payment-box ${s==='partial'?'paid':s}">
        <div class="payment-box-month">${ML[mo].slice(0,3)}</div>
        <div class="payment-box-amount">${a>0?fmt(a):'—'}</div>
      </div>`;}).join('')}
    </div>`;
  document.getElementById('detail-edit-btn').style.display=isAdmin()?'':'none';
  document.getElementById('detail-edit-btn').onclick=()=>{closeModal('modal-detail');openEditMember(id);};
  openModal('modal-detail');
}

/* ══════════════════════════════════════════════════════
   PAYMENT
══════════════════════════════════════════════════════ */
function openPayment(id){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const m=_members.find(x=>x.id===id);if(!m)return;
  document.getElementById('payment-modal-title').textContent=`Payment — ${esc(m.name)}`;
  document.getElementById('pay-member-id').value=id;
  document.getElementById('pay-total').value=m.deposit;
  previewSplit();openModal('modal-payment');
}
function previewSplit(){
  const val=parseInt(document.getElementById('pay-total').value)||0;
  const sp=splitDep(val);
  document.getElementById('split-preview').innerHTML=`
    <div style="font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.08em;color:var(--text3);margin-bottom:8px">Split Preview</div>
    <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:6px">
      ${MONTHS.map(mo=>{const a=sp[mo],s=depStatus(a);const ok=s==='paid'||s==='partial';
        return`<div style="background:${ok?'var(--paid-bg)':'var(--unpaid-bg)'};border-radius:7px;padding:8px 4px;text-align:center;border:1px solid ${ok?'#b2ddd1':'var(--border)'}">
          <div style="font-size:9px;font-weight:700;color:${ok?'var(--paid)':'var(--text3)'};text-transform:uppercase;margin-bottom:3px">${ML[mo].slice(0,3)}</div>
          <div style="font-size:11px;font-family:'DM Mono',monospace;color:${ok?'var(--paid)':'var(--text3)'}">${a>0?fmt(a):'—'}</div>
        </div>`;}).join('')}
    </div>`;
}
async function savePayment(){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  const id=parseInt(document.getElementById('pay-member-id').value);
  const dep=parseInt(document.getElementById('pay-total').value)||0;
  showLoader(true);
  try{
    await dbUpdate('members',{id},{deposit:dep});
    toast('💳 Payment saved');closeModal('modal-payment');
    await fetchAll();renderMembers();renderDashboard();
  }catch(e){toast('❌ Failed to save payment');console.error(e);}
  showLoader(false);
}

/* ══════════════════════════════════════════════════════
   EXPORT
══════════════════════════════════════════════════════ */
function exportCSV(){
  if(!isAdmin()){toast('🔒 Admin only');return;}
  closeExportMenu();
  const M=[..._members].sort((a,b)=>b.deposit-a.deposit);
  const h=['#','Name','Phone','Role','Type','Total',...MONTHS.map(m=>ML[m])];
  const rows=M.map((m,i)=>{const sp=splitDep(m.deposit);return[i+1,m.name,m.phone,m.role,m.type,m.deposit,...MONTHS.map(mo=>sp[mo])].join(',');});
  const csv=[h.join(','),...rows].join('\n');
  const a=document.createElement('a');
  a.href=URL.createObjectURL(new Blob([csv],{type:'text/csv'}));
  a.download='UMOJA_WVJ_'+new Date().toISOString().slice(0,10)+'.csv';
  a.click();toast('📄 CSV exported');
}
function exportPrint(){if(!isAdmin()){toast('🔒 Admin only');return;}closeExportMenu();setTimeout(()=>window.print(),200);}
function toggleExportMenu(){document.getElementById('export-menu').classList.toggle('open');}
function closeExportMenu(){document.getElementById('export-menu').classList.remove('open');}
document.addEventListener('click',e=>{if(!e.target.closest('.export-wrap'))closeExportMenu();});

/* ══════════════════════════════════════════════════════
   MODALS
══════════════════════════════════════════════════════ */
function openModal(id){document.getElementById(id).classList.add('open');}
function closeModal(id){document.getElementById(id).classList.remove('open');}
document.querySelectorAll('.modal-overlay').forEach(o=>{
  o.addEventListener('click',e=>{if(e.target===o)o.classList.remove('open');});
});

/* ══════════════════════════════════════════════════════
   TOAST
══════════════════════════════════════════════════════ */
let _tt;
function toast(msg){
  const ex=document.querySelector('.toast');if(ex)ex.remove();clearTimeout(_tt);
  const el=document.createElement('div');el.className='toast';
  el.textContent=msg;
  document.body.appendChild(el);_tt=setTimeout(()=>el.remove(),2800);
}

/* ══════════════════════════════════════════════════════
   EXPOSE TO GLOBAL — required for type="module" scope
══════════════════════════════════════════════════════ */
Object.assign(window,{
  doLogin,doLogout,
  showView,toggleSidebar,closeSidebar,setBnav,
  handleTopbarAdd,handleFab,
  renderMembers,renderDashboard,renderEventsList,
  openAddMember,openEditMember,saveMember,askDeleteMember,viewMemberDetail,
  openPayment,savePayment,previewSplit,
  openAddEvent,openEditEvent,saveEvent,askDeleteEvent,
  openEventDetail,backToEvents,toggleContrib,
  exportCSV,exportPrint,toggleExportMenu,closeExportMenu,
  openModal,closeModal,
});

/* ══════════════════════════════════════════════════════
   INIT — restore session if valid, else show login
══════════════════════════════════════════════════════ */
(async()=>{
  const { data:{ session } } = await supabase.auth.getSession();
  if(session){
    const role=session.user?.user_metadata?.role;
    if(role==='admin'||role==='member'){
      _currentUser=session.user; _currentRole=role;
      document.getElementById('login-screen').classList.remove('active');
      applyRoleUI(role);
      startInactivityWatcher();
      await fetchAll();
      renderDashboard();
      return;
    }
  }
  document.getElementById('login-screen').classList.add('active');
  setTimeout(()=>document.getElementById('login-email')?.focus(),200);
})();
</script>
</body>
</html>
