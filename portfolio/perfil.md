# Nahuel Gómez Suárez

**Full stack developer — Mar del Plata, Argentina**

> Sistemas en producción, no demos.

Un SaaS multi-tenant con clientes pagando hoy, la plataforma que sostiene dos
ecommerce reales y sistemas de gestión modelados sobre cómo trabaja cada negocio
de verdad.

**Disponible para nuevas oportunidades.**

---

## Contacto

| | |
|---|---|
| Email | gomezsuareznahuel01@gmail.com |
| LinkedIn | https://www.linkedin.com/in/gomeznahuel |
| GitHub | https://github.com/nauelGomez |
| CV | [Nahuel-Gomez-Suarez-CV.pdf](https://nahuelgomez.pro/Nahuel-Gomez-Suarez-CV.pdf) |
| Ubicación | Mar del Plata, Buenos Aires, Argentina |

---

## Cómo trabaja

No armo demos. Armo cosas que otra gente abre todas las mañanas para trabajar.

Diseño y construyo el sistema completo: modelo de datos, API, integraciones de
pago y despliegue. Después lo mantengo mientras el cliente lo usa, que es donde
se ve si estaba bien hecho.

Me interesa el momento en que un sistema deja de ser un proyecto y pasa a ser
algo de lo que alguien depende para trabajar.

---

## Sistemas en producción

Tres sistemas, los tres corriendo ahora mismo.

### 01 · mëtalix

**Producto propio · En producción**

SaaS multi-tenant de gestión para chatarrerías, construido de punta a punta.

- **Problema.** Las chatarrerías gestionan turnos, pesajes y pagos con planillas
  o sistemas armados a mano para cada negocio. No hay forma de escalar ni de dar
  de alta un cliente nuevo rápido.
- **Qué hice.** El producto completo, backend y frontend, con aislamiento de
  datos verificado en tres capas de código y tests, y panel de administración
  para altas, planes, roles y pagos por suscripción.
- **Resultado.** En producción, con clientes activos pagando hoy. Sumar un
  negocio es darlo de alta, no desplegar otra instancia.

**Construido con:** TypeScript · Express 5 · Prisma · PostgreSQL · React 19

Incluye calendario de logística con turnos, rutas y seguimiento en una sola
vista, y panel multi-tenant donde cada negocio tiene su plan y sus usuarios
sobre la misma base de código.

### 02 · Sastre

**Plataforma propia · 2 tiendas activas**

La plataforma de ecommerce multi-tienda sobre la que hoy corren dos negocios
reales.

- **Problema.** Cada tienda nueva significaba levantar otro servidor, otra base
  y otro mantenimiento en paralelo. No escalaba.
- **Qué hice.** Una sola API con su panel, pensada para que abrir una tienda sea
  darla de alta, no montar infraestructura. Stock por variante y carga masiva de
  catálogo por Excel.
- **Resultado.** Dos tiendas activas sobre la misma base: Suburbia, con dominio
  propio y vendiendo, y Play Zone Mar del Plata.

**Construido con:** Node · Express · Prisma · PostgreSQL · Railway

**Tiendas en línea:**
- Suburbia — https://suburbiauy.com (dominio propio, vendiendo)
- Play Zone — Mar del Plata

Stock por variante (talle y color con su propio inventario) y exportación de
reportes CSV con plantillas.

### 03 · Truck and Drinks & Barbac

**Por contrato · En uso**

Dos sistemas de gestión a medida, construidos sobre el proceso real de cada
negocio.

- **Problema.** Negocios operando con planillas y software genérico que no
  refleja cómo trabajan realmente: stock, eventos y presupuestos en un caso,
  gestión interna en el otro.
- **Qué hice.** Relevé el proceso real de cada negocio y lo modelé en el
  sistema, no al revés. Truck and Drinks corre motores de cálculo propios para
  stock, eventos y presupuestos.
- **Resultado.** Los dos en uso activo por sus clientes, con mantenimiento y
  nuevas funciones a pedido.

**Construido con:** PHP / Symfony · Symfony 8 · Angular · MongoDB · PostgreSQL ·
AWS con Docker · Railway

Incluye depósitos e inventario en tiempo real y recomendaciones logísticas con
investigación operativa avanzada: rutas, cargas y tiempos óptimos por evento.

---

## Stack

**Backend y datos**
Node.js (Express) · PHP (Laravel, Symfony) · APIs REST · WebSockets, Socket.io ·
Arquitectura multi-tenant · PostgreSQL (Prisma) · MongoDB · MySQL

**Frontend**
React · Angular · Astro · TypeScript

**Infraestructura e integraciones**
Docker · AWS (EC2, S3) · Railway · Fly.io · GitHub Actions ·
WhatsApp (Baileys) con bots conversacionales · Mercado Pago · Meta CAPI

---

## Además de los productos propios

Trabajo full-time migrando sistemas que no pueden darse el lujo de frenar:
relevar lo que ya existe, migrarlo sin cortar el servicio y dejarlo documentado
para el resto del equipo. Ahí es donde se nota si el modelo de datos estaba bien
pensado.

---

## Datos

| | |
|---|---|
| **Educación** | Técnico superior en análisis, desarrollo y programación de aplicaciones — ISET, Mar del Plata (2022–2024) |
| **Idiomas** | Español nativo · inglés B2 (certificado) |
| **Disponibilidad** | Presencial en Mar del Plata, jornada completa |

---

Estoy abierto a nuevas oportunidades. Contame qué están construyendo y te
respondo: gomezsuareznahuel01@gmail.com

*Versión en inglés: [/profile.md](https://nahuelgomez.pro/profile.md) · Última actualización: 2026-09-08*
