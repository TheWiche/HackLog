# HackLog // Offensive Security & Red Team Field Notes
> **Universidad de La Guajira — Facultad de Ingeniería**  
> **Asignatura:** Hacking Ético & Seguridad Ofensiva (2026-II)  
> **Docente:** Luis Ángel Ramírez Mendoza  
> **Auditores:**  
> - Nelson Wilinton Cotes Yepez (Cód. 0182210015)  
> - Carlos Andrés Martínez Jáuregui (Cód. 0002620001)

---

## 🛡️ Descripción de la Plataforma HackLog
**HackLog** es un portal interactivo y bitácora técnica de seguridad ofensiva estructurada para documentar paso a paso evaluaciones de pentesting, laboratorios CTF y análisis de vulnerabilidades web, diseñado con una arquitectura modular para alojar futuras auditorías y prácticas.

### Módulos del Portal:
- 📁 **Corte 1 — CTF Web & Post-Explotación [Completado]:**
  - **Sitio 1 (TechNova Store - P80):** Inyección SQL booleana y UNION-based, cracking MD5 con John the Ripper, subida de webshell con bypass de Content-Type a PDF, RCE y escalada de privilegios a root mediante binario SUID y PATH Hijacking (`netdiag`).
  - **Sitio 2 (Larm182 Solutions - P8080):** Fuga de información en `phpinfo()`, fuerza bruta a formularios con THC-Hydra, control de acceso roto (IDOR) en actas de infraestructura, y carga de webshell mediante HTTP PUT en Burp Suite.
- 📁 **Corte 2 — Infraestructura, Redes & Active Directory [Próximamente]:** Pivoting, Kerberoasting, BloodHound y evaluación de dominios internos.
- 📁 **Corte 3 — Explotación Binaria & Hardening [Próximamente]:** Buffer overflow, ROP chains, shellcoding e ingeniería inversa.

---

## 🚀 Despliegue en Vivo (Live Demo)
Puedes consultar el portal interactivo y la documentación completa en línea a través de GitHub Pages:  
👉 **[Acceder a HackLog en Vivo](https://TheWiche.github.io/HackLog/)**

---

## 🏆 Resumen de Flags Obtenidas (Corte 1)

| Objetivo | Vector / Técnica | Flag / Credencial Recuperada | Ubicación en el Servidor |
| :--- | :--- | :--- | :--- |
| **Sitio 1 (FLAG 1)** | Webshell RCE (www-data) | `FLAG{6e2c3a325feda8c8283908fba329969}` | `/var/www/technova/flag1.txt` |
| **Sitio 1 (FLAG 2)** | Escalada Root (SUID / PATH) | `FLAG{53dbcc8c5acc828c0ae1e085e575f25d}` | `/var/www/technova/.private/flag2.txt` |
| **Sitio 2 (FLAG)** | IDOR Reporte #73 | `C0rp0r4t3_B4ckup_2026` | Usuario `hacking_etico2026` |

---

## ⚖️ Marco Legal & Ética Profesional
Todas las pruebas de penetración documentadas en este repositorio se realizaron exclusivamente en entornos controlados con fines académicos de acuerdo con:
- **Ley 1273 de 2009 (Colombia):** Tipificación de delitos informáticos (Arts. 269A - 269F).
- **Ley 1581 de 2012 (Habeas Data):** Protección y custodia de datos personales.
