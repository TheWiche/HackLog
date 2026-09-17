# CTF: Reconocimiento, Explotación y Análisis de Vulnerabilidades Web
> **Universidad de La Guajira — Facultad de Ingeniería**  
> **Asignatura:** Hacking Ético & Seguridad Ofensiva (2026-II)  
> **Docente:** Luis Ángel Ramírez Mendoza  
> **Estudiante:** Nelson Wilinton Cotes Yepez (Cód. 0182210015)

---

## 🛡️ Descripción del Proyecto
Portal técnico y bitácora interactiva de auditoría de seguridad sobre dos escenarios web vulnerables en laboratorio de evaluación:
- **Sitio 1 — TechNova Store (Puerto 80):** E-commerce vulnerable a SQLi UNION-based, cracking de credenciales MD5, bypass de Content-Type en carga de archivos para RCE y escalada de privilegios a root mediante binarios SUID y PATH Hijacking.
- **Sitio 2 — Larm182 Solutions (Puerto 8080):** Plataforma corporativa con fuga de información en diagnóstico `phpinfo()`, ataque de fuerza bruta a login con THC-Hydra, control de acceso roto (IDOR) en actas de infraestructura, y carga de webshell mediante el método HTTP PUT con Burp Suite.

---

## 🚀 Despliegue en Vivo (Live Demo)
Puedes consultar el portal interactivo y la documentación completa en línea a través de GitHub Pages:  
👉 **[Ver Guía Nelson Cotes Online](https://TheWiche.github.io/ethical-hacking-ctf-guide/)**

---

## 📂 Estructura del Repositorio
```text
├── assets/
│   └── images/            # 35 Capturas de pantalla forenses del laboratorio
├── index.html             # Aplicación web / portal interactivo de documentación
├── generate_portal.py     # Script generador de la plataforma web
├── README.md              # Documentación técnica general
```

---

## 🏆 Resumen de Flags Obtenidas

| Objetivo | Vector / Técnica | Flag / Credencial Recuperada | Ubicación en el Servidor |
| :--- | :--- | :--- | :--- |
| **Sitio 1 (FLAG 1)** | Webshell RCE (www-data) | `FLAG{6e2c3a325feda8c8283908fba329969}` | `/var/www/technova/flag1.txt` |
| **Sitio 1 (FLAG 2)** | Escalada Root (SUID / PATH) | `FLAG{53dbcc8c5acc828c0ae1e085e575f25d}` | `/var/www/technova/.private/flag2.txt` |
| **Sitio 2 (FLAG)** | IDOR Reporte #73 | `C0rp0r4t3_B4ckup_2026` | Usuario `hacking_etico2026` |

---

## ⚖️ Marco Legal & Ética Profesional
Todas las pruebas de penetración documentadas en este repositorio se realizaron exclusivamente en entornos controlados con autorización explícita para fines académicos de acuerdo con:
- **Ley 1273 de 2009 (Colombia):** Tipificación de delitos informáticos (Arts. 269A - 269F).
- **Ley 1581 de 2012 (Habeas Data):** Protección y custodia de datos personales.

