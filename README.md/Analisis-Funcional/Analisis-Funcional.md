# Análisis Funcional – Pool Pay

**Proyecto:** Pool Pay – Plataforma de Pagos con Criptomonedas  
**Fecha:** 30/07/2025  
**Versión:** 1.0.0

**Autores:**

* Functional Analyst: Alexis Mauriz  
* Product Manager: Alexis Mauriz  
* Full Stack Developer: A Difinir

---

## Índice

1. [Introducción](#introducción)  
   * [Propósito del Documento](#propósito-del-documento)  
   * [Alcance](#alcance)

2. [Visión General del Producto](#visión-general-del-producto)  
   * [Objetivos del Sistema](#objetivos-del-sistema)  
   * [Público Objetivo](#público-objetivo)  
   * [Alcance Funcional](#alcance-funcional)

3. [Perfiles de Usuario y Roles](#perfiles-de-usuario-y-roles)

4. [Descripción General](#descripción-general)  
   * [Funciones Principales](#funciones-principales)  
   * [Limitaciones y Supuestos](#limitaciones-y-supuestos)

5. [Perspectiva Técnica](#perspectiva-técnica)  
   * [Stack Tecnológico](#stack-tecnológico)  
   * [Arquitectura del Sistema](#arquitectura-del-sistema)  
   * [Modelado de Datos Resumido](#modelado-de-datos-resumido)

6. [Requisitos](#requisitos)  
   * [Casos de Uso](#casos-de-uso)  
   * [Requisitos Funcionales](#requisitos-funcionales)  
   * [Requisitos No Funcionales](#requisitos-no-funcionales)  
   * [Requisitos de Diseño](#requisitos-de-diseño)

7. [Especificaciones de Proceso](#especificaciones-de-proceso)  
   * [Registro e Identidad Verificada](#registro-e-identidad-verificada)  
   * [Proceso de Compra](#proceso-de-compra)

8. [Atributos de Calidad del Sistema](#atributos-de-calidad-del-sistema)

9. [Seguridad y Autenticación](#seguridad-y-autenticación)

10. [Roadmap de Desarrollo](#roadmap-de-desarrollo)

11. [Glosario](#glosario)

12. [Anexos](#anexos)

---

## 1. Introducción

### Propósito del Documento

Este documento define los requisitos funcionales y no funcionales, así como la arquitectura y los procesos críticos de **Pool Pay**, plataforma de pagos con criptomonedas B2C y C2C, para asegurar un desarrollo alineado a objetivos de negocio y experiencia de usuario.

### Alcance

Cubre módulos de registro, autenticación, compra, sistema de referidos, notificaciones y soporte interno, sin incluir integraciones externas de pasarelas tradicionales.

## 2. Visión General del Producto

### Objetivos del Sistema

1. Reducir pasos de compra a ≤ 3 clics (checkout express).  
2. Garantizar transferencias < 1 minuto con hash rastreable.  
3. Incentivar adopción mediante comisiones del 0.5 % y programa de referidos.  
4. Priorizar privacidad y validación automática de red.

### Público Objetivo

* Usuarios sin cuenta bancaria (checkout sin registro).  
* Freelancers y compradores recurrentes (geolocalización).  
* Comercios locales interesados en comercios criptográficos.

### Alcance Funcional

* Registro opcional y completo con KYC/2FA.  
* Compra y pago con múltiples criptomonedas (BTC, USDT, USDC).  
* Panel de referidos con generación de enlaces y recompensas.  
* Geolocalización de productos.  
* Alertas internas para soporte y métricas.

## 3. Perfiles de Usuario y Roles

| Rol                 | Permisos Principales                                            |
| ------------------- | --------------------------------------------------------------- |
| **Comprador**       | Explorar productos, pagar con wallet, ver historial             |
| **Vendedor**        | Configurar redes cripto, listar productos, gestionar stock      |
| **Administrador**   | Validar KYC, gestionar usuarios, ver alertas de soporte         |
| **Soporte Técnico** | Recibir alertas en tiempo real, acceder al historial de errores |

## 4. Descripción General

### Funciones Principales

* **Checkout Express**: Compra sin registro mínimo.  
* **Gestión de KYC/2FA**: Validaciones condicionales según estado.  
* **Filtrado Geográfico**: Productos ordenados por proximidad.  
* **Sistema de Referidos**: Enlaces únicos y recompensas en USDT.  
* **Notificaciones y Alertas**: Emails, push y panel interno.

### Limitaciones y Supuestos

* Sin pasarelas de pago FIAT integradas.  
* Conexión a Internet estable.  
* Consentimiento explícito para geolocalización.

## 5. Perspectiva Técnica

### Stack Tecnológico

* **Frontend:** React.  
* **Backend:** Node.js (Express).  
* **Base de Datos:** PostgreSQL.  
* **Generación de PDF:** Puppeteer o similar.  
* **Notificaciones:** Email (SendGrid/SES) y push.

### Arquitectura del Sistema

Se compone de un cliente SPA en React que consume APIs REST del backend Express. La base de datos PostgreSQL almacena usuarios, transacciones, referidos y logs. Un servicio de workers gestiona alertas y validación de blockchain.

### Modelado de Datos Resumido

* **Usuarios** (id, nombre, email, estado_KYC, red_pref).  
* **Productos** (id, vendedor_id, red, precio, ubicación).  
* **Transacciones** (id, usuario_id, producto_id, hash, estado, fecha).  
* **Referidos** (id, usuario_origen, usuario_referido, recompensa).

## 6. Requisitos

### Casos de Uso

* Registro e Identidad Verificada (CuO1)  
* Inicio de Sesión y Tutorial Onboarding (CuO2/CuO9)  
* Proceso de Compra con validación de red (CuO3/CuO6)  
* Notificación post-KYC (CuO4)  
* Geolocalización de Productos (CuO5)  
* Alertas para Soporte (CuO7)  
* Sistema de Referidos (CuO8)

### Requisitos Funcionales

1. **RF001 – Registro sin cuenta** (US‑001).  
2. **RF002 – Checkout con wallet** (US‑001, US‑003).  
3. **RF003 – Validación de red y hash** (US‑004, US‑005).  
4. **RF004 – Geolocalización de productos** (US‑003).  
5. **RF005 – Panel de referidos** (US‑008).  
6. **RF006 – Alertas internas** (US‑007).  
7. **RF007 – Tutorial Onboarding** (US‑006, US‑009).

### Requisitos No Funcionales

* **RNF001 – Rendimiento:** Responder < 500 ms en endpoints críticos.  
* **RNF002 – Disponibilidad:** 99.5 % uptime.  
* **RNF003 – Seguridad:** HTTPS, JWT, bcrypt, protección CSRF/XSS.  
* **RNF004 – Escalabilidad:** Servicios desacoplados y horizontalizables.

### Requisitos de Diseño

* UI responsive sin exceso de JavaScript.  
* UX fluido: flows simplificados a ≤ 3 pasos.  
* Accesibilidad WCAG 2.1.

## 7. Especificaciones de Proceso

### Registro e Identidad Verificada

Ver flujo ampliado en Caso de Uso 1: KYC biométrico, email, 2FA condicional.

### Proceso de Compra

Flujo detallado en Caso de Uso 3: selección, dirección, validación de red, confirmación de pago y generación de recibo/PDF.

## 8. Atributos de Calidad del Sistema

* **Seguridad:** KYC, cifrado y roles.  
* **Rendimiento:** Transacciones < 1 minuto.  
* **Usabilidad:** Checkout express y tutorial.  
* **Portabilidad:** Desplegable en Windows, Linux, macOS.  
* **Mantenibilidad:** Código modular, pruebas unitarias.

## 9. Seguridad y Autenticación

* JWT para sesión.  
* 2FA tras KYC aprobado.  
* Middleware de permisos.

## 10. Roadmap de Desarrollo

| Sprint | Duración  | Hito                                   |
| ------ | --------- | -------------------------------------- |
| 1      | 2 semanas | Infraestructura, registro y KYC        |
| 2      | 2 semanas | Checkout express y validación de red   |
| 3      | 2 semanas | Geolocalización y tutorial onboarding  |
| 4      | 2 semanas | Sistema de referidos y alertas soporte |
| 5      | 2 semanas | Pruebas E2E, optimización y deploy     |

## 11. Glosario

* **KYC:** Know Your Customer.  
* **2FA:** Two Factor Authentication.  
* **Hash:** Identificador de transacción blockchain.

## 12. Anexos

* Diagramas UML y Flujo (Mermaid).  
* DER completo en PostgreSQL.  
* Especificación JSON de endpoints REST. 

#### Diagrama UML
![Diagrama U.M.L.](./Diagramas/U.M.L.drawio.png)

#### Diagrama de Flujo
![Diagrama de Flujo (DF)](./Diagramas/D.F.drawio.png)

#### Diagrama Entidad Relacion
![Diagrama DER](./Diagramas/D.E.R..png)

