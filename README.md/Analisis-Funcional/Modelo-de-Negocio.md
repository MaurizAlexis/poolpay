# Índice - Modelo de Negocio Pool Pay

## Secciones Principales

1. [Descripción General](#descripción-general)
2. [Objetivos del Sistema](#objetivos-del-sistema)
3. [Público Objetivo](#público-objetivo)
4. [Funcionalidades Principales](#funcionalidades-principales)
5. [Automatizaciones Inteligentes](#automatizaciones-inteligentes)
6. [Stack Tecnológico](#stack-tecnológico)
7. [Modelo de Negocios](#modelo-de-negocios)
8. [Roadmap Inicial](#roadmap-inicial)
9. [Conclusión](#conclusión)

## Sistema CRUD

10. [Endpoints Clave](#sistema-crud-endpoints-clave)

    * [Usuarios](#usuarios)
    * [Transacciones](#transacciones)
    * [Referidos](#referidos)

## Componentes Estratégicos

11. [Ventajas Competitivas](#ventajas-competitivas)
12. [Conclusión Final](#conclusión-final)
13. [Modelo de Datos Extendido](#modelo-de-datos-extendido)

---

## Descripción General

**Pool Pay** es una plataforma de pagos con criptomonedas que agiliza transacciones B2C y C2C, eliminando fricciones en KYC/2FA y priorizando privacidad. Ofrece:

* Checkout express con registro (US-001).
* Sistema de referidos con recompensas en USDT (US-008).
* Validación automática de redes blockchain (US-004).
* Soporte para múltiples wallets (BTC, USDT, USDC).

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Objetivos del Sistema

1. **Conversión:** Reducir pasos en compras (≤3 clics).
2. **Adopción:** Incentivar comercios con bajas comisiones (0.5% vs 2-3% tradicional).
3. **Seguridad:** Transacciones <1 minuto con hash rastreable (US-005).
4. **Crecimiento:** Viralidad mediante programa de referidos (US-008).

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Público Objetivo

| Segmento               | Necesidad                          | Ejemplo Real (Entrevista)  |
| ---------------------- | ---------------------------------- | -------------------------- |
| **Usuarios sin banco** | Pagar sin cuentas tradicionales    | Nadine Barros (Lemon Cash) |
| **Freelancers**        | Recibir pagos globales en cripto   | Devs remotos en Latam      |
| **Comercios locales**  | Reducir costos por pagos digitales | Tiendas de electrónicos    |

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Funcionalidades Principales

* Registro opcional para checkout express.
* Múltiples monedas: BTC, USDT, USDC.
* Programa de referidos automatizado.
* Conversor de divisas cripto en tiempo real.
* Historial y hash de transacciones.

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Automatizaciones Inteligentes

* **Validación de red automática:** evita errores de envío.
* **Verificación de hash en blockchain:** seguimiento instantáneo.
* **Descuentos automáticos para referidos.**

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Stack Tecnológico

* **Frontend:** React.
* **Backend:** JavaScript.
* **DB:** SQLPostgre.

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Modelo de Negocios

* **Freemium para usuarios.**
* **Comisión del 0.5% para comercios.**
* **Licencia mensual para comercios que deseen funciones extra.**
* **Recompensas con sistema de puntos y referidos.**

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Roadmap Inicial

* **Q3 2024:** Desarrollo MVP y validación técnica.
* **Q4 2024:** Alianzas con comercios y usuarios testers.
* **Q1 2025:** Expansión LATAM.
* **Q2 2025:** Escalado global y soporte multilenguaje.

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Conclusión

Una plataforma pensada para el futuro del dinero digital. Simple, segura y sin fricciones.

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Sistema CRUD (Endpoints Clave)

### Usuarios

```json
POST   /users           → Crear usuario (KYC opcional)
GET    /users/:id       → Obtener perfil + historial
PUT    /users/wallet    → Actualizar wallet preferida

POST   /tx              → Crear nueva transacción
GET    /tx/:id          → Detalle de transacción + hash

POST   /referrals       → Crear referido
GET    /referrals/user  → Obtener mis referidos y recompensas
```

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Ventajas Competitivas

* **Privacy-first:** Si requiere KYC para transacciones pequeñas (US-001).
* **Multi-red:** Evita errores con tooltips interactivos (US-004).
* **Gamificación:** Recompensas en USDT impulsan crecimiento (US-008).
* **Comunicación Directa:** Interacción fluida entre usuarios, comercios y administradores.
* **Adaptación:** Perfiles y flujos adaptados al tipo de producto.
* **Accesibilidad:** Modelo de pago accesible para pymes e individuos.
* **Escalabilidad:** Expansión prevista a comunidades de nicho, provincias y países.

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Conclusión Final

**Cryptonita-BT** no es solo una pasarela de pagos, sino un **ecosistema** que combina:
Experiencia sin fricciones + Incentivos alineados + Escalabilidad técnica.

*Meta Q4 2024:* Procesar \$1M USD mensuales en transacciones.

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)

---

## Modelo de Datos Extendido

### Listado de Entidades

**Usuario (ED)**

* ID\_Usuario (PK)
* Nombre de Usuario
* Teléfono del Usuario
* Perfil Profesional (expertise en producción de productos y servicios)
* Estado de Miembro (activo, inactivo)
* Nombre de la Empresa UK
* Descripción
* Localidad (PK)
* Pais
* Número de Cuenta

**Producto (ED)**

* ID\_Producto (PK)
* Localidad (PK)
* Nombre del Producto
* Rubro del Producto
* Pais
* Precio
* Descripción
* Número de Cuenta

**Servicios (ED)**

* ID\_Servicio (PK)
* Localidad (PK)
* Nombre del Servicio
* Rubro del Producto
* Pais
* Precio
* Descripción
* Número de Cuenta

**Roles (ED)**

* ID\_Usuario (PK)
* Nombre del Usuario (FK)
* Descripción

### Relaciones

* Un Usuario puede ofertar muchos Productos/Servicios (1 a M).
* Un Usuario puede vender muchos Productos/Servicios (1 a M).
* Un Administrador puede organizar múltiples Publicaciones (1 a M).
* Unos Administradores pueden coordinar muchos Traslados de Productos (M a M).

[Volver al índice](#índice---modelo-de-negocio-Pool Pay)
