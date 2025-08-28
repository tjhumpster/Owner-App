<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, viewport-fit=cover" />
  
  <!-- PWA & iOS specific meta tags -->
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="apple-mobile-web-app-title" content="Chalet CRM">
  <meta name="theme-color" content="#131E29">
  <meta name="mobile-web-app-capable" content="yes">
  
  <title>Chalet Owners CRM</title>
  
  <!-- PWA Manifest -->
  <link rel="manifest" href="data:application/json;base64,ewogICJuYW1lIjogIkNoYWxldCBPd25lcnMgQ1JNIiwKICAic2hvcnRfbmFtZSI6ICJDaGFsZXQgQ1JNIiwKICAiZGlzcGxheSI6ICJzdGFuZGFsb25lIiwKICAib3JpZW50YXRpb24iOiAicG9ydHJhaXQiLAogICJzdGFydF91cmwiOiAiLyIsCiAgImJhY2tncm91bmRfY29sb3IiOiAiI0Y4RjhGOCIsCiAgInRoZW1lX2NvbG9yIjogIiMxMzFFMjkiLAogICJpY29ucyI6IFsKICAgIHsKICAgICAgInNyYyI6ICJkYXRhOmltYWdlL3BuZztiYXNlNjQsaVZCT1J3MEtHZ29BQUFBTlNVaEVVZ0FBQUhBQUFBQndDQVlBQUFBOUlpUEFBQUFCRWxFUVZSb1ErVmNBR29BQUFBTFkwZkVBQUFBQVhSU1RsTUFRT2JZWmdBQUFBQkpSVTVFcmtKZ2dnPT0iLAogICAgICAic2l6ZXMiOiAiMTEyeDExMiIsCiAgICAgICJ0eXBlIjogImltYWdlL3BuZyIKICAgIH0sCiAgICB7CiAgICAgICJzcmMiOiAiZGF0YTppbWFnZS9wbmc7YmFzZTY0LGlWQk9SdzBLR2dvQUFBQU5TVWhFVWdBQUFJQUFBQUNBQ0FZQUFBQlJ1M1Y5QUFBQkJFbEVRVlI0MnUzY0FXb0FBQUJNWTBmRUFBQUFBWFJTVGxNQVFPYllaZ0FBQUFCSlJVNUVya0pnZ2c9PSIsCiAgICAgICJzaXplcyI6ICIxMjh4MTI4IiwKICAgICAgInR5cGUiOiAiaW1hZ2UvcG5nIgogICAgfSwKICAgIHsKICAgICAgInNyYyI6ICJkYXRhOmltYWdlL3BuZztiYXNlNjQsaVZCT1J3MEtHZ29BQUFBTlNVaEVVZ0FBQUlBQUFBQ0FDQVlBQUFCUnUzVjlBQUFCQkVsRVFWUjQydTNjQVdvQUFBQk1ZMGZFQUFBQUFYUlNUbE1BUU9iWVpnQUFBQUJKUlU1RXJrSmdnZz09IiwKICAgICAgInNpemVzIjogIjE5MngxOTIiLAogICAgICAidHlwZSI6ICJpbWFnZS9wbmciCiAgICB9LAogICAgewogICAgICAic3JjIjogImRhdGE6aW1hZ2UvcG5nO2Jhc2U2NCxpVkJPUncwS0dnb0FBQUFOU1VoRVVnQUFBUUFBQUFFQUNBWUFBQUR3RlNOcEFBQUJCRWxFUVZSNDJ1M2NBV29BQUFCUVkwZkVBQUFBQVhSU1RsTUFRT2JZWmdBQUFBQkpSVTVFcmtKZ2dnPT0iLAogICAgICAic2l6ZXMiOiAiMjU2eDI1NiIsCiAgICAgICJ0eXBlIjogImltYWdlL3BuZyIKICAgIH0sCiAgICB7CiAgICAgICJzcmMiOiAiZGF0YTppbWFnZS9wbmc7YmFzZTY0LGlWQk9SdzBLR2dvQUFBQU5TVWhFVWdBQUFnQUFBQUlBQ0FZQUFBQzdXQ1RrQUFBQkJFbEVRVlI0MnUzY0FXb0FBQUJRWTBmRUFBQUFBWFJTVGxNQVFPYllaZ0FBQUFCSlJVNUVya0pnZ2c9PSIsCiAgICAgICJzaXplcyI6ICI1MTJ4NTEyIiwKICAgICAgInR5cGUiOiAiaW1hZ2UvcG5nIgogICAgfQogIF0KfQ==">
  
  <!-- Apple Touch Icons -->
  <link rel="apple-touch-icon" href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAABRu3V9AAABBElEQVR42u3cAWoAAABMY0fEAAAAXRSTlMAQObYZgAAAABJRU5ErkJggg==">
  
  <link href="https://fonts.googleapis.com/css2?family=Sen:wght@400;600;700&display=swap" rel="stylesheet">
  
  <style>
    :root{
      /* Brand */
      --navy:#131E29; --sand:#D7D2CB; --slate:#3F4443; --ice:#F8F8F8;
      --forest:#385542; --gold:#D7A048; --lime:#E3EABA; --cream:#F5E1A4;
      /* UI */
      --bg:var(--ice); --text:#101418; --muted:#6B7280; --card:#ffffff;
      --radius:18px; --shadow:0 10px 30px rgba(0,0,0,.08);
    }
    *{box-sizing:border-box}
    html,body{height:100%;overscroll-behavior-y:contain}
    body{margin:0;font-family:'Sen',system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial,sans-serif;background:var(--bg);color:var(--text);padding-top:env(safe-area-inset-top);padding-bottom:env(safe-area-inset-bottom)}
    .app{display:grid;grid-template-columns:280px 1fr;min-height:100vh}
    aside{background:var(--navy);color:#fff;display:flex;flex-direction:column;gap:16px;padding:24px;position:sticky;top:0;height:100vh;z-index:100}
    .brand{font-weight:700;font-size:20px;letter-spacing:.5px;display:flex;align-items:center;gap:10px}
    .brand img{height:26px;filter:brightness(0) invert(1)}
    nav{display:flex;flex-direction:column;gap:8px;margin-top:16px}
    .nav-btn{display:flex;align-items:center;gap:10px;padding:12px 14px;border-radius:12px;border:none;background:transparent;color:#fff;font-weight:600;cursor:pointer;-webkit-tap-highlight-color:transparent}
    .nav-btn:hover,.nav-btn.active{background:rgba(255,255,255,.1)}
    .spacer{flex:1}
    .logout{margin-top:auto;background:rgba(255,255,255,.08)}

    header{display:flex;align-items:center;justify-content:space-between;padding:18px 24px;background:linear-gradient(180deg,#fff,rgba(255,255,255,.7));backdrop-filter:saturate(140%) blur(6px);position:sticky;top:0;z-index:10;border-bottom:1px solid #eee}
    .pill{background:#eef1f4;padding:8px 12px;border-radius:999px;font-weight:700;color:#1f2937;border:1px solid #e5e7eb}

    main{padding:24px;display:grid;gap:24px;position:relative;z-index:1}
    .grid{display:grid;grid-template-columns:repeat(12,1fr);gap:24px}
    .card{background:var(--card);border-radius:var(--radius);box-shadow:var(--shadow);padding:18px;position:relative}
    .card h3{margin:0 0 12px 0}
    .kpi{display:flex;align-items:center;justify-content:space-between}
    .kpi .value{font-size:28px;font-weight:800}

    /* Tokens */
    .token{display:inline-flex;align-items:center;gap:6px;padding:6px 10px;border-radius:999px;border:1px solid #e5e7eb;background:#f6f7f9;color:#111;font-weight:700}

    /* Calendar - Fixed z-index issues */
    .calendar-wrap{display:grid;grid-template-columns:2fr 1fr;gap:24px;position:relative;z-index:1}
    .calendar{display:grid;gap:10px}
    .cal-header{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:10px}
    .cal-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:8px}
    .day-name{font-weight:800;color:var(--slate);text-align:center}
    .cal-cell{background:#fff;border:1px solid #eee;border-radius:12px;min-height:86px;padding:8px;position:relative;cursor:pointer;-webkit-tap-highlight-color:transparent}
    .cal-cell .date{font-weight:700;font-size:13px;color:var(--slate)}
    .bar{position:absolute;left:6px;right:6px;height:8px;border-radius:6px;bottom:8px;background:var(--forest);opacity:.85}
    .bar.holiday{background:var(--gold)}

    .toolbar{display:flex;gap:8px;flex-wrap:wrap}
    .btn{border:none;border-radius:12px;padding:10px 12px;font-weight:700;cursor:pointer;-webkit-tap-highlight-color:transparent;-webkit-appearance:none;appearance:none}
    .btn.primary{background:var(--forest);color:#fff}
    .btn.ghost{background:#eceff3}
    .btn.warning{background:var(--gold)}
    .btn.biometric{background:linear-gradient(135deg, #667eea 0%, #764ba2 100%);color:#fff}

    .list{display:flex;flex-direction:column;gap:10px}
    .row{display:flex;align-items:center;justify-content:space-between;background:#fff;border-radius:14px;padding:14px;border:1px solid #eee}
    .row .sub{color:var(--muted);font-size:13px}

    .listing{display:grid;grid-template-columns:160px 1fr;gap:16px;align-items:center}
    .listing img{width:160px;height:110px;object-fit:cover;border-radius:12px}

    .hidden{display:none}

    /* Auth cover */
    .auth{position:fixed;inset:0;background:linear-gradient(135deg,var(--navy),#0e1722);display:flex;align-items:center;justify-content:center;z-index:9999}
    .auth .panel{width:min(420px,92vw);background:#fff;border-radius:22px;box-shadow:var(--shadow);padding:26px;text-align:center}
    .auth .subtitle{color:#4b5563;margin:0 0 20px 0}
    .auth input{width:100%;padding:12px 14px;border:1px solid #e5e7eb;border-radius:12px;-webkit-appearance:none;appearance:none}

    /* Toast */
    .toast{position:fixed;bottom:calc(18px + env(safe-area-inset-bottom));right:18px;background:#111;color:#fff;border-radius:12px;padding:12px 14px;opacity:0;transform:translateY(10px);transition:.25s;z-index:200;pointer-events:none}
    .toast.show{opacity:1;transform:translateY(0);pointer-events:auto}

    /* Modal */
    #modal.hidden{display:none}
    #modal{position:fixed;inset:0;background:rgba(0,0,0,.35);display:flex;align-items:center;justify-content:center;z-index:150;padding:env(safe-area-inset-top) env(safe-area-inset-right) env(safe-area-inset-bottom) env(safe-area-inset-left)}
    #modal .inner{width:min(760px,92vw);max-height:86vh;overflow:auto}

    /* PWA Install prompt */
    .install-prompt{position:fixed;bottom:calc(80px + env(safe-area-inset-bottom));left:50%;transform:translateX(-50%);background:var(--navy);color:#fff;border-radius:16px;padding:16px 20px;box-shadow:0 12px 28px rgba(0,0,0,.25);z-index:300;display:none;animation:slideUp 0.3s ease}
    .install-prompt.show{display:block}
    @keyframes slideUp{from{transform:translateX(-50%) translateY(20px);opacity:0}to{transform:translateX(-50%) translateY(0);opacity:1}}

    @media (max-width:1080px){
      .app{grid-template-columns:1fr}
      aside{position:fixed;left:0;top:0;bottom:0;transform:translateX(-100%);transition:.25s ease;z-index:200;width:280px}
      aside.open{transform:translateX(0);box-shadow:10px 0 30px rgba(0,0,0,.2)}
      header .menu{display:inline-block}
      header .brand-inline{display:flex;align-items:center;gap:10px}
      main{padding:16px}
      .calendar-wrap{grid-template-columns:1fr}
      .grid{grid-template-columns:1fr}
      .card{grid-column:span 1 !important}
    }
    @media (min-width:1081px){ header .menu{display:none} }
    
    /* iOS specific adjustments */
    @supports (-webkit-touch-callout: none) {
      input, textarea, select {font-size:16px}
    }
  </style>
</head>
<body>
  <!-- Auth overlay with biometric -->
  <div id="auth" class="auth">
    <div class="panel">
      <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Ccircle cx='50' cy='50' r='40' fill='%23131E29'/%3E%3Ctext x='50' y='60' text-anchor='middle' fill='white' font-size='30' font-weight='bold'%3ECRM%3C/text%3E%3C/svg%3E" alt="CRM" style="height:60px;margin-bottom:16px">
      <h2>Chalet Owner Portal</h2>
      <p class="subtitle">Secure access to your dashboard</p>
      <div style="display:grid;gap:10px;">
        <button class="btn biometric" id="biometricBtn" onclick="attemptBiometric()">🔐 Use Face ID / Touch ID</button>
        <div style="position:relative;margin:10px 0;">
          <div style="position:absolute;left:0;right:0;top:50%;height:1px;background:#e5e7eb"></div>
          <span style="background:#fff;padding:0 10px;position:relative;color:#6b7280;font-size:14px">or sign in with email</span>
        </div>
        <input id="email" placeholder="Email" type="email" autocomplete="email"/>
        <input id="pw" placeholder="Password" type="password" autocomplete="current-password"/>
        <button class="btn ghost" onclick="mockLogin()">Sign In</button>
      </div>
      <p class="sub" style="color:#6b7280;margin-top:8px;font-size:12px">Demo mode - any credentials work</p>
    </div>
  </div>

  <!-- PWA Install Prompt -->
  <div id="installPrompt" class="install-prompt">
    <div style="font-weight:700;margin-bottom:4px">Install Chalet CRM</div>
    <div style="font-size:14px;opacity:0.9">Add to your home screen for the best experience</div>
    <div style="display:flex;gap:10px;margin-top:12px">
      <button class="btn primary" onclick="installPWA()" style="flex:1">Install</button>
      <button class="btn ghost" onclick="dismissInstall()" style="background:rgba(255,255,255,0.1);color:#fff">Later</button>
    </div>
  </div>

  <div class="app" id="app" aria-hidden="true">
    <aside id="sidebar" aria-label="Sidebar">
      <div class="brand">
        <svg width="26" height="26" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
          <circle cx="50" cy="50" r="40" fill="white"/>
          <path d="M50 20 L70 40 L70 70 L30 70 L30 40 Z" fill="#131E29"/>
          <rect x="40" y="50" width="20" height="20" fill="white"/>
        </svg>
        Chalet CRM
      </div>
      <nav id="nav">
        <button class="nav-btn active" data-target="dashboard">📊 Dashboard</button>
        <button class="nav-btn" data-target="calendar">📅 Calendar</button>
        <button class="nav-btn" data-target="reports">📈 Reports</button>
        <button class="nav-btn" data-target="listings">🏠 Listings</button>
        <button class="nav-btn" data-target="documents">📄 Documents</button>
        <button class="nav-btn" data-target="blog">📝 Blog</button>
        <button class="nav-btn" data-target="chat">💬 Chatbot</button>
        <button class="nav-btn" data-target="settings">⚙️ Settings</button>
      </nav>
      <div class="spacer"></div>
      <button class="nav-btn logout" onclick="logout()">🚪 Logout</button>
    </aside>

    <div>
      <header>
        <div class="brand-inline">
          <button class="btn ghost menu" onclick="toggleSidebar()">☰</button>
          <span class="pill">Beta v2.0</span>
        </div>
        <div style="display:flex;align-items:center;gap:10px">
          <span style="color:var(--muted)">Welcome back!</span>
          <div style="width:36px;height:36px;border-radius:50%;background:linear-gradient(135deg,#667eea,#764ba2)"></div>
        </div>
      </header>

      <main>
        <!-- DASHBOARD -->
        <section id="dashboard" class="grid" data-section>
          <div class="card" style="grid-column:span 8">
            <h3>Upcoming bookings</h3>
            <div class="list" id="upcomingList"></div>
          </div>
          <div class="card" style="grid-column:span 4">
            <div class="kpi">
              <div>
                <div class="value" id="kpiRevenue">€—</div>
                <div class="sub">Projected revenue (next 30d)</div>
              </div>
              <div class="token" id="kpiChange">+4.2%</div>
            </div>
            <hr style="border:none;border-top:1px solid #eee;margin:16px 0">
            <div class="toolbar">
              <button class="btn primary" onclick="downloadICS()">Export calendar</button>
              <button class="btn ghost" onclick="openSection('reports')">View reports</button>
            </div>
          </div>

          <div class="card" style="grid-column:span 7">
            <h3>Listing quality</h3>
            <p class="sub">How your main chalet performs across OTAs</p>
            <div class="row">
              <strong>Photos</strong><span class="sub">12/15 recommended</span>
              <span class="token">80%</span>
            </div>
            <div class="row">
              <strong>Description</strong><span class="sub">1,240 characters</span>
              <span class="token">72%</span>
            </div>
            <div class="row">
              <strong>Amenities</strong><span class="sub">Hot tub, Sauna, Ski-in/out</span>
              <span class="token">92%</span>
            </div>
          </div>

          <div class="card" style="grid-column:span 5">
            <h3>Quick actions</h3>
            <div class="toolbar">
              <button class="btn primary" onclick="openSection('listings')">Preview listing</button>
              <button class="btn warning" onclick="flagListing()">Flag issue</button>
              <button class="btn ghost" onclick="openSection('documents')">Policies</button>
            </div>
          </div>
        </section>

        <!-- CALENDAR -->
        <section id="calendar" class="hidden" data-section>
          <div class="calendar-wrap">
            <div class="card">
              <div class="cal-header">
                <div class="toolbar">
                  <button class="btn ghost" onclick="prevMonth()">◀</button>
                  <h3 id="calTitle" style="margin:0 8px"></h3>
                  <button class="btn ghost" onclick="nextMonth()">▶</button>
                </div>
                <div class="toolbar">
                  <label><input type="checkbox" id="toggleHolidays" checked onchange="renderCalendar()"> Holidays</label>
                  <label><input type="checkbox" id="toggleBookings" checked onchange="renderCalendar()"> Bookings</label>
                </div>
              </div>
              <div class="cal-grid" id="calGrid"></div>
              <div class="toolbar" style="margin-top:12px">
                <button class="btn primary" onclick="downloadICS()">Export .ics</button>
                <button class="btn ghost" onclick="tip('Calendar exported!')">Sync calendars</button>
              </div>
            </div>
            <div class="card">
              <h3>Day details</h3>
              <div id="dayDetails" class="list"><div class="sub">Select a day to see bookings.</div></div>
              <hr style="border:none;border-top:1px solid #eee;margin:16px 0">
              <h3>Upcoming (30 days)</h3>
              <div class="list" id="upcomingSide"></div>
            </div>
          </div>
        </section>

        <!-- REPORTS -->
        <section id="reports" class="hidden" data-section>
          <div class="card">
            <h3>Financial reports</h3>
            <div class="list" id="reportList"></div>
          </div>
        </section>

        <!-- LISTINGS -->
        <section id="listings" class="hidden" data-section>
          <div class="card">
            <h3>My listing</h3>
            <div class="listing">
              <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 160 110'%3E%3Crect fill='%23e5e7eb' width='160' height='110'/%3E%3Cpath d='M80 30 L100 50 L100 80 L60 80 L60 50 Z' fill='%23131E29'/%3E%3Crect x='70' y='60' width='20' height='20' fill='white'/%3E%3C/svg%3E" alt="Chalet"/>
              <div>
                <h4>Chalet Mont Brillant</h4>
                <p class="sub">Val d'Isère • 5BR • Hot tub • Sleeps 12</p>
                <div class="toolbar">
                  <button class="btn ghost" onclick="tip('Opening website...')">View on Website</button>
                  <button class="btn ghost" onclick="tip('Opening Airbnb...')">Airbnb</button>
                  <button class="btn warning" onclick="flagListing()">Flag issue</button>
                </div>
              </div>
            </div>
          </div>
        </section>

        <!-- DOCUMENTS -->
        <section id="documents" class="hidden" data-section>
          <div class="card">
            <h3>Documents & policies</h3>
            <div class="list">
              <div class="row"><div><strong>Security deposit policy</strong><div class="sub">Guidelines for amounts & disputes</div></div><button class="btn ghost" onclick="openDoc('security')">Open</button></div>
              <div class="row"><div><strong>Damage process</strong><div class="sub">What to do when things break</div></div><button class="btn ghost" onclick="openDoc('damage')">Open</button></div>
              <div class="row"><div><strong>Cleaning checklist</strong><div class="sub">Standards and vendor contacts</div></div><button class="btn ghost" onclick="openDoc('clean')">Open</button></div>
            </div>
          </div>
        </section>

        <!-- BLOG -->
        <section id="blog" class="hidden" data-section>
          <div class="card">
            <h3>Owner resources</h3>
            <div class="list" id="blogList"></div>
          </div>
        </section>

        <!-- CHATBOT -->
        <section id="chat" class="hidden" data-section>
          <div class="card">
            <h3>Assistant</h3>
            <div id="chatWindow" style="border:1px solid #eee;border-radius:14px;height:280px;overflow:auto;padding:12px;background:#fff"></div>
            <div style="display:flex;gap:8px;margin-top:8px">
              <input id="chatInput" placeholder="Ask a question..." style="flex:1;padding:12px 14px;border:1px solid #e5e7eb;border-radius:12px"/>
              <button class="btn primary" onclick="sendChat()">Send</button>
              <button class="btn warning" onclick="escalate()">Escalate</button>
            </div>
          </div>
        </section>

        <!-- SETTINGS -->
        <section id="settings" class="hidden" data-section>
          <div class="card">
            <h3>Settings</h3>
            <div class="list">
              <div class="row"><div><strong>Biometric Login</strong><div class="sub" id="biometricStatus">Not configured</div></div><button class="btn ghost" onclick="setupBiometric()">Setup</button></div>
              <div class="row"><div><strong>Calendar sync</strong><div class="sub">Export .ics for external calendars</div></div><button class="btn ghost" onclick="openSection('calendar')">Open</button></div>
              <div class="row"><div><strong>App version</strong><div class="sub">PWA v2.0 Beta</div></div><button class="btn ghost" onclick="checkUpdate()">Check updates</button></div>
            </div>
          </div>
        </section>

      </main>
    </div>
  </div>

  <div id="toast" class="toast" role="status" aria-live="polite"></div>

  <!-- Modal -->
  <div id="modal" class="hidden">
    <div class="card inner">
      <div style="display:flex;align-items:center;justify-content:space-between;gap:16px">
        <h3 id="modalTitle">Title</h3>
        <button class="btn ghost" onclick="closeModal()">✕</button>
      </div>
      <div id="modalBody" style="margin-top:8px"></div>
    </div>
  </div>

  <script>
    // ============ SERVICE WORKER & PWA ============
    if ('serviceWorker' in navigator) {
      navigator.serviceWorker.register('data:text/javascript;base64,Ly8gU2VydmljZSBXb3JrZXIgZm9yIENoYWxldCBDUk0gUFdBCmNvbnN0IENBQ0hFX05BTUUgPSAnY2hhbGV0LWNybS12MScKY29uc3QgdXJsc1RvQ2FjaGUgPSBbJy8nXQoKc2VsZi5hZGRFdmVudExpc3RlbmVyKCdpbnN0YWxsJywgZSA9PiB7CiAgZS53YWl0VW50aWwoY2FjaGVzLm9wZW4oQ0FDSEVfTkFNRSkudGhlbihjID0+IGMuYWRkQWxsKHVybHNUb0NhY2hlKSkpCn0pCgpzZWxmLmFkZEV2ZW50TGlzdGVuZXIoJ2ZldGNoJywgZSA9PiB7CiAgZS5yZXNwb25kV2l0aChjYWNoZXMubWF0Y2goZS5yZXF1ZXN0KS50aGVuKHIgPT4gciB8fCBmZXRjaChlLnJlcXVlc3QpKSkKfSk=').catch(e => console.log('SW registration failed'));
    }

    // PWA install prompt
    let deferredPrompt;
    window.addEventListener('beforeinstallprompt', (e) => {
      e.preventDefault();
      deferredPrompt = e;
      if (!sessionStorage.getItem('installDismissed')) {
        setTimeout(() => document.getElementById('installPrompt').classList.add('show'), 2000);
      }
    });

    function installPWA() {
      if (deferredPrompt) {
        deferredPrompt.prompt();
        deferredPrompt.userChoice.then((result) => {
          if (result.outcome === 'accepted') {
            tip('App installed successfully!');
          }
          deferredPrompt = null;
        });
      }
      document.getElementById('installPrompt').classList.remove('show');
    }

    function dismissInstall() {
      sessionStorage.setItem('installDismissed', '1');
      document.getElementById('installPrompt').classList.remove('show');
    }

    // ============ BIOMETRIC AUTHENTICATION ============
    const AUTH_KEY = 'chaletCRM_auth';
    const CRED_KEY = 'chaletCRM_credId';
    
    // Check if biometric is available
    async function checkBiometricSupport() {
      if (!window.PublicKeyCredential) return false;
      try {
        const available = await PublicKeyCredential.isUserVerifyingPlatformAuthenticatorAvailable();
        return available;
      } catch {
        return false;
      }
    }

    // Setup biometric authentication
    async function setupBiometric() {
      try {
        const supported = await checkBiometricSupport();
        if (!supported) {
          tip('Biometric auth not available on this device');
          return;
        }

        // Create credential
        const challenge = new Uint8Array(32);
        crypto.getRandomValues(challenge);
        
        const publicKeyCredentialCreationOptions = {
          challenge,
          rp: { name: "Chalet CRM", id: window.location.hostname || "localhost" },
          user: {
            id: new TextEncoder().encode("user@chaletcrm"),
            name: "user@chaletcrm",
            displayName: "Chalet Owner"
          },
          pubKeyCredParams: [{alg: -7, type: "public-key"}],
          authenticatorSelection: {
            authenticatorAttachment: "platform",
            userVerification: "required"
          },
          timeout: 60000,
          attestation: "direct"
        };

        const credential = await navigator.credentials.create({
          publicKey: publicKeyCredentialCreationOptions
        });

        // Store credential ID
        const credId = btoa(String.fromCharCode(...new Uint8Array(credential.rawId)));
        sessionStorage.setItem(CRED_KEY, credId);
        sessionStorage.setItem(AUTH_KEY, '1');
        
        document.getElementById('biometricStatus').textContent = 'Face ID / Touch ID enabled';
        tip('Biometric authentication enabled!');
      } catch (err) {
        console.error('Biometric setup failed:', err);
        tip('Failed to setup biometric auth');
      }
    }

    // Attempt biometric login
    async function attemptBiometric() {
      try {
        const supported = await checkBiometricSupport();
        if (!supported) {
          tip('Using demo mode - biometric not available');
          mockLogin();
          return;
        }

        // For demo purposes, we'll simulate biometric auth
        // In production, you'd verify against stored credentials
        const btn = document.getElementById('biometricBtn');
        btn.textContent = '⏳ Authenticating...';
        btn.disabled = true;

        // Simulate biometric prompt
        setTimeout(() => {
          sessionStorage.setItem(AUTH_KEY, '1');
          enterApp();
        }, 1500);

      } catch (err) {
        console.error('Biometric auth failed:', err);
        tip('Authentication failed. Please use email/password.');
        document.getElementById('biometricBtn').disabled = false;
        document.getElementById('biometricBtn').textContent = '🔐 Use Face ID / Touch ID';
      }
    }

    // ============ DEMO DATA ============
    const bookings = [
      { id:1, title:'Family – Smith', start:'2025-02-20', end:'2025-02-24', price:1850 },
      { id:2, title:'Corporate Retreat', start:'2025-03-12', end:'2025-03-16', price:4200 },
      { id:3, title:'Easter Week', start:'2025-04-19', end:'2025-04-26', price:5200 },
      { id:4, title:'Summer – Jones', start:'2025-08-10', end:'2025-08-17', price:4600 }
    ];

    const frHolidays2025 = [
      '2025-01-01','2025-04-21','2025-05-01','2025-05-08','2025-05-29','2025-06-09','2025-07-14','2025-08-15','2025-11-01','2025-11-11','2025-12-25'
    ];
    const ukHolidays2025 = [
      '2025-01-01','2025-04-18','2025-04-21','2025-05-05','2025-05-26','2025-08-25','2025-12-25','2025-12-26'
    ];
    const schoolWindows2025 = [
      ['2025-02-15','2025-03-03'], ['2025-04-12','2025-04-28'], ['2025-10-18','2025-11-03'], ['2025-12-20','2026-01-05']
    ];

    const reports = [
      {name:'Balance Sheet – Q1 2025', type:'balance', amount: '€12,550'},
      {name:'Tax Summary – FY 2024', type:'tax', amount: '€8,120'},
      {name:'Revenue Detail – Last 30 days', type:'rev', amount: '€6,980'}
    ];

    const posts = [
      {title:'Maximising winter occupancy', url:'#', excerpt:'Pricing strategies and minimum stays…'},
      {title:'Hot tub maintenance guide', url:'#', excerpt:'Daily checks, weekly shock, filters…'},
      {title:'OTA channel management', url:'#', excerpt:'Airbnb vs Booking vs direct bookings…'}
    ];

    // ============ AUTH ============
    function mockLogin() { 
      sessionStorage.setItem(AUTH_KEY, '1'); 
      enterApp(); 
    }
    
    function logout() { 
      sessionStorage.clear();
      location.reload(); 
    }

    function enterApp() {
      document.getElementById('auth').style.display = 'none';
      document.getElementById('app').ariaHidden = 'false';
      init();
    }

    // Check if already logged in
    if (sessionStorage.getItem(AUTH_KEY)) {
      document.getElementById('auth').style.display = 'none';
      document.getElementById('app').ariaHidden = 'false';
    }

    // ============ NAVIGATION ============
    function toggleSidebar() { 
      document.getElementById('sidebar').classList.toggle('open'); 
    }
    
    function openSection(id) {
      document.querySelectorAll('[data-section]').forEach(s => s.classList.add('hidden'));
      document.getElementById(id).classList.remove('hidden');
      document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
      const btn = [...document.querySelectorAll('.nav-btn')].find(b => b.dataset.target === id);
      if (btn) btn.classList.add('active');
      window.scrollTo({top: 0, behavior: 'smooth'});
      
      // Close sidebar on mobile after navigation
      if (window.innerWidth <= 1080) {
        document.getElementById('sidebar').classList.remove('open');
      }
    }

    document.getElementById('nav').addEventListener('click', e => {
      if (e.target.matches('.nav-btn')) {
        openSection(e.target.dataset.target);
      }
    });

    // ============ DASHBOARD ============
    function renderDashboard() {
      const container = document.getElementById('upcomingList');
      container.innerHTML = '';
      const soon = [...bookings].sort((a,b) => a.start.localeCompare(b.start)).slice(0, 3);
      soon.forEach(b => {
        const el = document.createElement('div');
        el.className = 'row';
        el.innerHTML = `<div><strong>${b.title}</strong><div class="sub">${fmtRange(b.start, b.end)}</div></div><span class="token">${b.price.toLocaleString('fr-FR', {style: 'currency', currency: 'EUR'})}</span>`;
        container.appendChild(el);
      });
      
      const next30 = bookings.filter(b => daysBetween(new Date(), new Date(b.start)) <= 30).reduce((s, b) => s + b.price, 0);
      document.getElementById('kpiRevenue').textContent = next30.toLocaleString('fr-FR', {style: 'currency', currency: 'EUR'});
      document.getElementById('kpiChange').textContent = '+4.2%';
    }

    // ============ CALENDAR ============
    let calCursor = new Date();

    function prevMonth() { 
      calCursor.setMonth(calCursor.getMonth() - 1); 
      renderCalendar(); 
    }
    
    function nextMonth() { 
      calCursor.setMonth(calCursor.getMonth() + 1); 
      renderCalendar(); 
    }

    function within(d, start, end) { 
      return d >= start && d <= end; 
    }

    function renderCalendar() {
      const title = document.getElementById('calTitle');
      title.textContent = calCursor.toLocaleString('en-GB', {month: 'long', year: 'numeric'});
      const grid = document.getElementById('calGrid');
      grid.innerHTML = '';
      const y = calCursor.getFullYear(), m = calCursor.getMonth();
      const first = new Date(y, m, 1);
      const startDay = (first.getDay() + 6) % 7;
      const days = new Date(y, m + 1, 0).getDate();
      
      ['Mon','Tue','Wed','Thu','Fri','Sat','Sun'].forEach(d => {
        const h = document.createElement('div');
        h.className = 'day-name';
        h.textContent = d;
        grid.appendChild(h);
      });
      
      for (let i = 0; i < startDay; i++) {
        grid.appendChild(document.createElement('div'));
      }
      
      const showH = document.getElementById('toggleHolidays').checked;
      const showB = document.getElementById('toggleBookings').checked;
      
      for (let day = 1; day <= days; day++) {
        const cell = document.createElement('div');
        cell.className = 'cal-cell';
        const d = new Date(y, m, day);
        const iso = d.toISOString().slice(0, 10);
        const date = document.createElement('div');
        date.className = 'date';
        date.textContent = day;
        cell.appendChild(date);
        
        if (showB) {
          const any = bookings.some(b => within(d, new Date(b.start), new Date(b.end)));
          if (any) {
            const b = document.createElement('div');
            b.className = 'bar';
            cell.appendChild(b);
            cell.onclick = () => showDay(d);
          }
        }
        
        if (showH && (frHolidays2025.includes(iso) || ukHolidays2025.includes(iso) || schoolWindows2025.some(([s,e]) => within(d, new Date(s), new Date(e))))) {
          const h = document.createElement('div');
          h.className = 'bar holiday';
          h.style.height = '6px';
          h.style.bottom = '22px';
          cell.appendChild(h);
        }
        
        grid.appendChild(cell);
      }
      
      const upcoming = [...bookings].filter(b => daysBetween(new Date(), new Date(b.start)) >= 0 && daysBetween(new Date(), new Date(b.start)) <= 30).sort((a,b) => a.start.localeCompare(b.start));
      const side = document.getElementById('upcomingSide');
      side.innerHTML = '';
      (upcoming.length ? upcoming : bookings.slice(0, 3)).forEach(b => {
        const el = document.createElement('div');
        el.className = 'row';
        el.innerHTML = `<div><strong>${b.title}</strong><div class='sub'>${fmtRange(b.start, b.end)}</div></div><span class='token'>${b.price.toLocaleString('fr-FR', {style: 'currency', currency: 'EUR'})}</span>`;
        side.appendChild(el);
      });
    }

    function showDay(d) {
      const detail = document.getElementById('dayDetails');
      detail.innerHTML = '';
      const matches = bookings.filter(b => within(d, new Date(b.start), new Date(b.end)));
      if (matches.length === 0) {
        detail.innerHTML = '<div class="sub">No bookings for this day.</div>';
        return;
      }
      matches.forEach(b => {
        const el = document.createElement('div');
        el.className = 'row';
        el.innerHTML = `<div><strong>${b.title}</strong><div class='sub'>${fmtRange(b.start, b.end)}</div></div><span class='token'>${b.price.toLocaleString('fr-FR', {style: 'currency', currency: 'EUR'})}</span>`;
        detail.appendChild(el);
      });
    }

    function downloadICS() {
      const lines = ['BEGIN:VCALENDAR', 'VERSION:2.0', 'PRODID:-//Chalet CRM//EN'];
      bookings.forEach(b => {
        const dtStart = b.start.replace(/-/g, '');
        const dtEnd = addDays(new Date(b.end), 1).toISOString().slice(0, 10).replace(/-/g, '');
        lines.push('BEGIN:VEVENT');
        lines.push(`SUMMARY:${b.title}`);
        lines.push(`DTSTART;VALUE=DATE:${dtStart}`);
        lines.push(`DTEND;VALUE=DATE:${dtEnd}`);
        lines.push('END:VEVENT');
      });
      lines.push('END:VCALENDAR');
      const blob = new Blob([lines.join('\r\n')], {type: 'text/calendar'});
      const a = document.createElement('a');
      a.href = URL.createObjectURL(blob);
      a.download = 'chalet-bookings.ics';
      a.click();
      tip('Calendar exported! Import to your calendar app.');
    }

    // ============ REPORTS ============
    function renderReports() {
      const list = document.getElementById('reportList');
      list.innerHTML = '';
      reports.forEach(r => {
        const row = document.createElement('div');
        row.className = 'row';
        row.innerHTML = `<div><strong>${r.name}</strong><div class='sub'>${r.amount}</div></div>`;
        const actions = document.createElement('div');
        actions.style.display = 'flex';
        actions.style.gap = '8px';
        const viewBtn = btn('ghost', 'View', () => openReport(r));
        const dlBtn = btn('primary', 'Download', () => downloadCSV(r));
        actions.append(viewBtn, dlBtn);
        row.appendChild(actions);
        list.appendChild(row);
      });
    }

    function openReport(r) {
      showModal(r.name, `<div class='list'>
        <div class='row'><div><strong>Line items</strong><div class='sub'>Sample values</div></div><span class='token'>Demo</span></div>
        <div class='row'><div>Cleaning fees</div><div class='sub'>€420</div></div>
        <div class='row'><div>Maintenance</div><div class='sub'>€180</div></div>
        <div class='row'><div>Revenue</div><div class='sub'>${r.amount}</div></div>
      </div>`);
    }

    function downloadCSV(r) {
      const csv = 'name,amount\n' + r.name + ',' + r.amount + '\n';
      const blob = new Blob([csv], {type: 'text/csv'});
      const a = document.createElement('a');
      a.href = URL.createObjectURL(blob);
      a.download = r.name.replace(/\s+/g, '_') + '.csv';
      a.click();
      tip('Report downloaded!');
    }

    // ============ LISTINGS ============
    function flagListing() {
      tip('Issue flagged! Team will be notified.');
    }

    // ============ DOCUMENTS ============
    function openDoc(kind) {
      const map = {
        security: `<p><strong>Security deposits:</strong> Standard €800. Held as pre-auth for 7 days after checkout.</p>
                   <ul><li>Minor damage under €50: absorbed by ops budget.</li><li>Guest dispute: notify within 48h with evidence.</li></ul>`,
        damage: `<ol><li>Photograph and log the incident.</li><li>Get repair estimate from vendors.</li><li>Notify guest & insurance if needed.</li></ol>`,
        clean: `<p>Turnaround: 10:00–16:00. Checklist includes linens, hot tub, consumables, and sanitization.</p>`
      };
      showModal('Document', map[kind] || 'Document not found');
    }

    // ============ BLOG ============
    function renderBlog() {
      const list = document.getElementById('blogList');
      list.innerHTML = '';
      posts.forEach(p => {
        const row = document.createElement('div');
        row.className = 'row';
        row.innerHTML = `<div><strong>${p.title}</strong><div class='sub'>${p.excerpt}</div></div>`;
        const a = btn('ghost', 'Read', () => tip('Opening: ' + p.title));
        row.appendChild(a);
        list.appendChild(row);
      });
    }

    // ============ CHAT ============
    function pushChat(sender, msg) {
      const box = document.getElementById('chatWindow');
      const wrap = document.createElement('div');
      wrap.style.margin = '6px 0';
      wrap.innerHTML = `<div style="font-weight:700;color:${sender === 'You' ? '#111' : '#385542'}">${sender}</div><div>${msg}</div>`;
      box.appendChild(wrap);
      box.scrollTop = box.scrollHeight;
    }

    function sendChat() {
      const input = document.getElementById('chatInput');
      const q = input.value.trim();
      if (!q) return;
      pushChat('You', q);
      input.value = '';
      setTimeout(() => {
        pushChat('Assistant', cannedReply(q));
      }, 400);
    }

    function cannedReply(q) {
      q = q.toLowerCase();
      if (q.includes('deposit') || q.includes('damage')) return 'Security deposits are €800 pre-auth for 7 days. Check Documents for full policy.';
      if (q.includes('calendar') || q.includes('sync')) return 'Use Calendar → Export .ics for all calendar apps.';
      if (q.includes('tax')) return 'Tax summaries are under Reports. Download as CSV for your accountant.';
      return 'Lol get rekt m8';
    }

    function escalate() {
      tip('Escalated to team via Slack!');
    }

    // ============ UTILITIES ============
    function btn(kind, label, fn) {
      const b = document.createElement('button');
      b.className = 'btn ' + kind;
      b.textContent = label;
      b.onclick = fn;
      return b;
    }

    function tip(msg) {
      const t = document.getElementById('toast');
      t.textContent = msg;
      t.classList.add('show');
      setTimeout(() => t.classList.remove('show'), 2200);
    }

    function addDays(d, days) {
      const x = new Date(d);
      x.setDate(x.getDate() + days);
      return x;
    }

    function daysBetween(a, b) {
      return Math.ceil((new Date(b) - new Date(a)) / 86400000);
    }

    function fmtRange(s, e) {
      const ds = new Date(s), de = new Date(e);
      const opts = {day: 'numeric', month: 'short'};
      return `${ds.toLocaleDateString('en-GB', opts)}–${de.toLocaleDateString('en-GB', opts)}, ${de.getFullYear()}`;
    }

    function checkUpdate() {
      tip('You have the latest version!');
    }

    // ============ MODAL ============
    function showModal(title, html) {
      document.getElementById('modalTitle').textContent = title;
      document.getElementById('modalBody').innerHTML = html;
      document.getElementById('modal').classList.remove('hidden');
    }

    function closeModal() {
      document.getElementById('modal').classList.add('hidden');
    }

    document.getElementById('modal').addEventListener('click', (e) => {
      if (e.target.id === 'modal') closeModal();
    });

    // ============ INITIALIZATION ============
    function init() {
      renderDashboard();
      renderCalendar();
      renderReports();
      renderBlog();
      openSection('dashboard');
      
      // Check biometric support
      checkBiometricSupport().then(supported => {
        if (supported) {
          document.getElementById('biometricStatus').textContent = 'Available on this device';
        }
      });
    }

    if (sessionStorage.getItem(AUTH_KEY)) init();

    // iOS specific: Add to homescreen instructions
    if (/iPhone|iPad|iPod/.test(navigator.userAgent) && !window.navigator.standalone) {
      setTimeout(() => {
        if (!sessionStorage.getItem('iosInstructionShown')) {
          tip('Tap Share → Add to Home Screen for best experience');
          sessionStorage.setItem('iosInstructionShown', '1');
        }
      }, 3000);
    }
    // 👇 replace this with your real Slack webhook URL
    const SLACK_WEBHOOK_URL = https://hooks.slack.com/triggers/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;

    function flagListing(event) {
      // Find the listing card where the button was clicked
      const card = event.target.closest("#listings");
      const property = card.querySelector("h4")?.innerText || "Unknown property";
      const location = card.querySelector(".sub")?.innerText.split("•")[0].trim() || "Unknown location";
      const owner = prompt("Enter the owner's name:"); // quick input
      const accountManager = "Tom"; // fixed for now

      const payload = {
        text: `Hi! ${owner} has a problem with their listing.\nProperty - ${property}\nLocation - ${location}\nAccount manager - ${accountManager}`
      };

      fetch(SLACK_WEBHOOK_URL, {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify(payload)
      })
      .then(res => {
        if (res.ok) {
          alert("🚀 Issue flagged & sent to Slack!");
        } else {
          alert("⚠️ Failed to send message to Slack.");
        }
      })
      .catch(err => {
        console.error("Slack error:", err);
        alert("⚠️ Could not connect to Slack.");
      });
    }
  </script>
</body>
</html>
