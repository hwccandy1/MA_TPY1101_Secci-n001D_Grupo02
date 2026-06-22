# SRMM - Sistema de Reparación y Mantenimiento de Maquinaria

### Integrantes
Constanza Orellana - Corina Roa - Rocío Trujillo - Daniel Onetto 


![React](https://img.shields.io/badge/React-Frontend-blue)
![Node.js](https://img.shields.io/badge/Node.js-Backend-green)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue)
![Scrum](https://img.shields.io/badge/Metodolog%C3%ADa-Scrum-orange)
![Duoc UC](https://img.shields.io/badge/Duoc%20UC-Proyecto%20Acad%C3%A9mico-red)

## Descripción General

El **Sistema de Reparación y Mantenimiento de Maquinaria (SRMM)** es una plataforma web desarrollada para optimizar la gestión operativa y administrativa de maquinaria pesada utilizada en actividades industriales y de construcción.

El proyecto fue desarrollado para la empresa **Servicios Reparación y Mantención de Maquinarias Hermosilla y García Ltda.**, con el objetivo de digitalizar procesos críticos relacionados con el control de activos, mantenimientos preventivos, gestión de incidencias y administración de contratos de arriendo.

La solución permite centralizar la información operacional en una única plataforma, proporcionando trazabilidad, monitoreo en tiempo real y soporte para la toma de decisiones basada en datos.

---

## Objetivo del Proyecto

Diseñar e implementar una plataforma web que permita gestionar de forma centralizada la operación, mantenimiento y disponibilidad de maquinaria pesada, mejorando la eficiencia operacional y reduciendo los riesgos asociados a procesos manuales de administración.

---

## Problemática

Antes de la implementación de SRMM, la empresa gestionaba sus operaciones mediante registros físicos, anotaciones manuales y procesos informales.

Esta situación generaba diversos inconvenientes:

- Falta de visibilidad sobre el estado operativo de la maquinaria.
- Ausencia de control sobre mantenimientos preventivos.
- Riesgo de duplicidad en contratos de arriendo.
- Dificultades para generar reportes históricos.
- Incremento de tiempos de inactividad por fallas no planificadas.
- Limitaciones para la toma de decisiones estratégicas.

Como resultado, la organización operaba bajo un modelo reactivo que impactaba negativamente la disponibilidad de los equipos y la rentabilidad del negocio.

---

## Solución Propuesta

SRMM centraliza y automatiza la gestión de maquinaria mediante una plataforma web que permite:

- Controlar el inventario de equipos.
- Registrar horómetros y monitorear el uso de maquinaria.
- Automatizar alertas de mantenimiento preventivo.
- Gestionar incidencias técnicas.
- Administrar contratos de arriendo.
- Generar indicadores y reportes operacionales.
- Mantener trazabilidad completa de las operaciones.

---

## Funcionalidades Principales

### Gestión de Maquinaria

- Registro de equipos.
- Control de estados operacionales.
- Seguimiento de disponibilidad.
- Historial de utilización.

### ⏱️ Gestión de Horómetros

- Registro de horas de uso.
- Validación de lecturas.
- Historial cronológico.
- Seguimiento de desgaste operativo.

### Mantenimiento Preventivo

- Configuración de planes de mantención.
- Alertas automáticas.
- Bloqueo preventivo por uso excesivo.
- Registro de órdenes de trabajo.

### Gestión de Incidencias

- Registro de fallas.
- Clasificación por criticidad.
- Seguimiento de resolución.
- Historial técnico de equipos.

### Gestión de Arriendos

- Administración de contratos.
- Validación de disponibilidad.
- Prevención de solapamiento de fechas.
- Control de entrega y devolución.

### 📊 Dashboard y Reportes

- Indicadores operacionales.
- Estado de la flota.
- Alertas críticas.
- Estadísticas históricas.

---

## Arquitectura del Sistema

El sistema implementa una arquitectura **Monolítica Modular** basada en el patrón **Modelo-Vista-Controlador (MVC)**.

```text
┌──────────────────────┐
│      Frontend        │
│ React + Vite         │
└──────────┬───────────┘
           │ REST API
           ▼
┌──────────────────────┐
│      Backend         │
│ Node.js + Express    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│     PostgreSQL       │
│      Supabase        │
└──────────────────────┘
