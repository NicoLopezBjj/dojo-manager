# Dojo Manager — Product and Engineering Case Study

> **¿Preferís leerlo en castellano?** [La versión completa en castellano está más abajo.](#versión-en-castellano)

## Context

Dojo Manager began as a response to a concrete operational problem: running a jiu-jitsu academy required information spread across spreadsheets, messages, attendance notes, payment records, and manual calculations.

The objective was not simply to “digitize a spreadsheet.” It was to understand the academy’s actual rules and turn them into a product that reduces repetitive work, preserves history, and makes important decisions auditable.

## My role

I conceived, designed, and developed the product end to end:

- Discovery and translation of real operational needs into product rules.
- Information architecture and workflow design.
- Data modelling and historical traceability.
- Full-stack implementation.
- Security and permission boundaries.
- Production operation and iterative improvement.
- Preparation of an isolated, fictional portfolio demonstration.

## Product challenges

### Attendance is more than a checkbox

A student may physically attend while having an overdue payment or exceeding a monthly plan. The system preserves the real attendance while separately deciding whether it is eligible for teacher settlement. Authorized exceptions remain documented and reversible.

### Teacher payouts must be explainable

Teacher payments depend on valid collections and eligible attendance during a selected month. The product exposes the inputs behind the result so the calculation can be checked instead of behaving like an unexplained total.

### Corrections must not erase history

Payments, student status, plans, graduations, settlements, and operational exceptions can change. Where accountability matters, Dojo Manager keeps the previous context or an auditable correction instead of silently rewriting the past.

### Different users need different boundaries

Teachers need fast access to attendance, student creation, and received payments. They do not need settlements, configuration, financial summaries, or destructive administrative actions. The experience reflects that boundary and the server enforces it.

### Not every commercial workflow is a store

Academy apparel is produced through occasional campaigns. The product models campaign-specific products, costs, orders, partial payments, and deliveries without introducing unnecessary inventory or e-commerce complexity.

## Product approach

The work followed a few consistent principles:

1. Document the business rule before encoding it.
2. Prefer explicit workflows over generic abstractions.
3. Preserve information that explains financial and operational outcomes.
4. Keep the MVP focused on real recurring work.
5. Separate demonstration infrastructure and data from live operations.

## Engineering approach

The private application is a full-stack web product built with a typed relational model, server-side authorization, reusable operational components, and documented business rules.

Technical decisions were guided by maintainability rather than novelty:

- Relational data for connected operational history.
- Server-enforced permissions for sensitive actions.
- Deterministic fictional data for demonstrations.
- Reproducible calculations with inspectable inputs.
- Mobile-first operational workflows.
- Documentation treated as durable project memory.

## Outcome

Dojo Manager is used in the day-to-day operation of a real jiu-jitsu academy. It centralizes workflows that were previously fragmented and provides a foundation that can evolve from actual usage rather than speculation.

The public showcase intentionally contains no application source code or real organizational data. An isolated interactive demo is being prepared.

## What this project demonstrates

- Turning an ambiguous real-world process into a coherent product.
- Balancing usability, business rules, data integrity, and security.
- Delivering and operating a complete full-stack application.
- Making financial and operational behavior traceable.
- Maintaining scope while leaving room for evidence-based evolution.

---

# Versión en castellano

## Contexto

Dojo Manager nació como respuesta a un problema operativo concreto: administrar una academia de jiu-jitsu requería información distribuida entre planillas, mensajes, anotaciones de asistencia, registros de pagos y cálculos manuales.

El objetivo no era simplemente “digitalizar una planilla”. Era comprender las reglas reales de la academia y convertirlas en un producto que reduzca trabajo repetitivo, conserve historial y permita auditar decisiones importantes.

## Mi rol

Concebí, diseñé y desarrollé el producto de punta a punta:

- Descubrimiento y traducción de necesidades operativas reales en reglas de producto.
- Arquitectura de información y diseño de flujos.
- Modelado de datos y trazabilidad histórica.
- Implementación full-stack.
- Seguridad y límites de permisos.
- Operación productiva y mejora iterativa.
- Preparación de una demostración de portfolio aislada y ficticia.

## Desafíos de producto

### La asistencia es más que una casilla

Un alumno puede asistir físicamente aunque tenga una cuota vencida o haya superado el límite mensual. El sistema conserva la presencia real y decide por separado si corresponde incluirla en la liquidación docente. Las excepciones autorizadas quedan documentadas y pueden revertirse.

### Las liquidaciones deben poder explicarse

Los pagos docentes dependen de cobros válidos y asistencias computables de un mes. El producto muestra la información que origina el resultado para que pueda verificarse, en lugar de entregar un total inexplicable.

### Corregir no debe borrar la historia

Pagos, estados, planes, graduaciones, liquidaciones y excepciones pueden cambiar. Cuando importa la responsabilidad, Dojo Manager conserva el contexto anterior o una corrección auditable en lugar de reescribir silenciosamente el pasado.

### Cada usuario necesita límites diferentes

Los profesores necesitan acceso rápido a asistencias, alta de alumnos y pagos recibidos. No necesitan liquidaciones, configuración, resúmenes financieros ni acciones administrativas destructivas. La experiencia refleja ese límite y el servidor lo hace cumplir.

### No todo flujo comercial es una tienda

La indumentaria se produce mediante campañas ocasionales. El producto modela productos, costos, pedidos, pagos parciales y entregas por campaña sin introducir complejidad innecesaria de inventario o comercio electrónico.

## Enfoque de producto

El trabajo siguió principios consistentes:

1. Documentar la regla antes de convertirla en código.
2. Preferir flujos explícitos frente a abstracciones genéricas.
3. Conservar la información que explica resultados financieros y operativos.
4. Mantener el MVP enfocado en trabajo real y recurrente.
5. Separar datos e infraestructura de demostración de la operación real.

## Enfoque de ingeniería

La aplicación privada es un producto web full-stack con modelo relacional tipado, autorización en el servidor, componentes operativos reutilizables y reglas de negocio documentadas.

Las decisiones técnicas priorizaron mantenibilidad por encima de novedad:

- Datos relacionales para un historial operativo conectado.
- Permisos aplicados en el servidor para acciones sensibles.
- Datos ficticios determinísticos para demostraciones.
- Cálculos reproducibles con información inspeccionable.
- Flujos operativos mobile-first.
- Documentación como memoria duradera del proyecto.

## Resultado

Dojo Manager se utiliza en la operación cotidiana de una academia real de jiu-jitsu. Centraliza procesos antes fragmentados y ofrece una base que puede evolucionar a partir del uso real, no de especulación.

El showcase público no contiene código fuente de la aplicación ni datos reales. Se está preparando una demo interactiva aislada.

## Qué demuestra este proyecto

- Convertir un proceso real ambiguo en un producto coherente.
- Equilibrar usabilidad, reglas de negocio, integridad de datos y seguridad.
- Entregar y operar una aplicación full-stack completa.
- Hacer trazable el comportamiento financiero y operativo.
- Mantener el alcance y evolucionar a partir de evidencia.
