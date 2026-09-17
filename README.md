# HackLog // Security Operations & CTF Knowledge Base
> **Universidad de La Guajira — Facultad de Ingeniería**  
> **Asignatura:** Hacking Ético & Seguridad Ofensiva (2026-II)  
> **Docente:** Luis Ángel Ramírez Mendoza  
> **Mantenido por:** Nelson Cotes

---

## 🛡️ Descripción de la Plataforma HackLog
**HackLog** es un portal centralizado y catálogo interactivo de bitácoras técnicas de seguridad ofensiva, diseñado con una arquitectura multi-página para indexar evaluaciones de penetración web, laboratorios CTF y análisis forenses.

### 🌐 Arquitectura del Portal:
- 🏛️ **[HackLog Hub (Página Principal)](https://TheWiche.github.io/HackLog/):** Dashboard central con métricas globales de auditoría y catálogo de laboratorios completados.
- 🎯 **[Laboratorio 01: CTF Web & Post-Explotación](https://TheWiche.github.io/HackLog/laboratorio_1/):** Bitácora técnica exhaustiva del primer entorno evaluativo con 15 fases y 35 evidencias documentadas.
  - **Auditores:** Nelson Wilinton Cotes Yepez (Cód. 0182210015) & Carlos Andrés Martínez Jáuregui (Cód. 0002620001).

---

## 🏆 Resumen de Flags Obtenidas (Laboratorio 01)

| Objetivo | Vector / Técnica | Flag / Credencial Recuperada | Ubicación en el Servidor |
| :--- | :--- | :--- | :--- |
| **Sitio 1 (FLAG 1)** | Webshell RCE (`www-data`) | `FLAG{6e2c3a325feda8c8283908fba329969}` | `/var/www/technova/flag1.txt` |
| **Sitio 1 (FLAG 2)** | Escalada Root (SUID / PATH) | `FLAG{53dbcc8c5acc828c0ae1e085e575f25d}` | `/var/www/technova/.private/flag2.txt` |
| **Sitio 2 (FLAG)** | IDOR Reporte #73 | `C0rp0r4t3_B4ckup_2026` | Usuario `hacking_etico2026` |

---

## ⚖️ Marco Legal & Ética Profesional
Todas las pruebas de penetración documentadas en este repositorio se realizaron exclusivamente en entornos controlados con fines académicos de acuerdo con:
- **Ley 1273 de 2009 (Colombia):** Tipificación de delitos informáticos (Arts. 269A - 269F).
- **Ley 1581 de 2012 (Habeas Data):** Protección y custodia de datos personales.
