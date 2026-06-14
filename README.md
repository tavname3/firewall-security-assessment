# Proyecto de Hardening: Detección de Vulnerabilidades y Remediación en Firewall

## Descripción

Proyecto de seguridad en red que abarca el ciclo completo de evaluación y hardening sobre un entorno físico de firewall/NAT. Se realizaron pruebas de penetración activas, auditoría formal contra benchmarks CIS, aplicación de medidas de hardening y re-auditoría para validar la remediación.

Este laboratorio forma parte de un portafolio de proyectos de infraestructura y seguridad desarrollados previo a estadías de ingeniería.

---

## Objetivo

Identificar vulnerabilidades y debilidades de configuración en un firewall/NAT sobre hardware físico, documentar los hallazgos con evidencia técnica, aplicar remediaciones y verificar su efectividad mediante una segunda auditoría.

---

## Entorno del laboratorio

| Rol | Dispositivo | Sistema Operativo |
|---|---|---|
| Firewall / NAT (objetivo) | PC dedicada | Linux |
| Atacante | Kali Linux | Kali Linux Rolling |
| Administración / Documentación | Laptop | — |

**Topología:**

```
[Kali - Atacante] ──── LAN interna ──── [Firewall/NAT - Objetivo]
                                                  │
                                          [Laptop - Admin SSH]
```

> Todo el laboratorio opera en una red aislada y controlada. No se prueba infraestructura fuera del entorno de lab.

---

## Herramientas utilizadas

- **Nmap** — Escaneo de puertos, detección de servicios y OS fingerprinting
- **Metasploit** — Módulos auxiliares para análisis de vulnerabilidades
- **Wireshark / tcpdump** — Captura y análisis de tráfico de red
- **CIS Benchmarks** — Marco de referencia para auditoría formal

---

## Fases del proyecto

### [Fase 1 — Reconocimiento y escaneo activo](./01-reconocimiento/README.md)
Descubrimiento de hosts, escaneo de puertos y servicios, OS fingerprinting y captura de tráfico base.

### [Fase 2 — Explotación y análisis de vulnerabilidades](./02-explotacion/README.md)
Test de reglas NAT, intento de bypass de políticas, uso de módulos auxiliares de Metasploit y análisis de logs.

### [Fase 3 — Auditoría formal](./03-auditoria/README.md)
Verificación de configuraciones contra benchmarks CIS, clasificación de hallazgos por severidad y generación de evidencias.

### [Fase 4 — Hardening y remediación](./04-hardening/README.md)
Aplicación de correcciones sobre los hallazgos identificados, re-auditoría y comparativa antes/después.

---

## Reporte final

- [Reporte completo](./reporte-final/reporte.md)
- [Resumen ejecutivo](./reporte-final/executive-summary.md)

---

## Resultados clave

> *Esta sección se completará al finalizar el proyecto.*

---
## Autor
 
**Gustavo Isaias Nava Merino**  
TSU en Infraestructura de Redes Digitales  
Ingeniería en Redes Inteligentes y Ciberseguridad *(cursando)*  
Universidad Tecnológica de Puebla
