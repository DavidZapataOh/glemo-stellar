# Propuesta individual

**Nombre:** David Zapata

**Usuario de GitHub:** DavidZapataOh

---

## El problema

> El problema en una sola frase, sin mencionar blockchain.

La validación de documentos e información financiera es lenta, vulnerable al fraude y a la falsificación por inteligencia artificial, y obliga al usuario a exponer toda su información privada a terceros.

## ¿Quién lo sufre?

> Quién tiene el problema y en qué situación lo vive.

* **Entidades financieras, fintechs y rampas de pago (on/off ramps):** En el momento en que deben validar la solvencia, ingresos o titularidad de cuenta de un nuevo usuario o empresa para aprobar un crédito, abrir una cuenta o procesar pagos.
* **Usuarios y solicitantes:** Cada vez que deben compartir extractos bancarios completos o nóminas con intermediarios, exponiendo información sensible de sus transacciones y arriesgándose a filtraciones de datos.

## ¿Cómo se resuelve hoy y qué cuesta?

> Cómo lo resuelven hoy las personas afectadas y qué les cuesta en dinero, tiempo o esfuerzo.

* **Cómo se resuelve:** 
  1. El usuario descarga un extracto en PDF o toma capturas de pantalla y las sube a un portal o las envía por correo.
  2. La entidad recurre a revisión manual humana, herramientas de OCR básico o, si tiene suerte, a APIs centralizadas de Open Banking (que en la mayoría de países emergentes son caras, inestables o no existen).
* **Qué cuesta:**
  * **Tiempo:** Entre 1 a 4 días hábiles de fricción operativa, llamadas y esperas antes de dar una respuesta.
  * **Dinero y pérdidas:** Costos elevados en equipos de compliance/operaciones dedicados a cotejar papeles, y millones de dólares en pérdidas por fraude ante documentos manipulados con herramientas de diseño o IA generativa que los filtros tradicionales no detectan.
  * **Esfuerzo y fricción:** Tasas de abandono superiores al 40% en procesos de onboarding debido a la burocracia documental.

## ¿Por qué creo que blockchain podría aportar?

> Hipótesis personal, no certeza, apoyada en al menos un criterio de la Sesión 1: partes que no confían entre sí comparten un registro, histórico inalterable, o eliminar un intermediario que concentra la confianza.

El problema surge porque **partes que no confían entre sí** (la entidad financiera y el solicitante desconocido) se ven obligadas a depender de **intermediarios que concentran la confianza** (burós de crédito privados o validadores manuales) o a creer en documentos fácilmente manipulables.

Blockchain podría aportar valor al actuar como un **registro compartido, inalterable y auditable** donde se asientan atestaciones o pruebas criptográficas de validez en lugar de almacenar documentos en texto plano. Esto permitiría que cualquier entidad compruebe al instante si una condición financiera se cumple, eliminando el intermediario centralizado y garantizando un histórico a prueba de alteraciones sin comprometer la privacidad del usuario.