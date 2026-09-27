# Problem Brief

## Decisión del problema

### Problema elegido

> El problema ganador en una frase, sin mencionar blockchain, y quién lo propuso.

La validación de documentos e información financiera es lenta, vulnerable al fraude y a la falsificación por inteligencia artificial, y obliga al usuario a exponer toda su información privada a terceros.

### Por qué elegimos este

> Qué inclinó al equipo por este problema frente a los demás, según los criterios de la Sesión 1.

Este problema cumple de forma directa con los criterios de pertinencia de la Sesión 1:
1. **Partes que no confían entre sí:** El solicitante y la entidad financiera no se conocen y tienen incentivos contrapuestos (uno busca la aprobación inmediata; el otro, mitigar el riesgo de incumplimiento).
2. **Eliminación de intermediarios centralizados:** Hoy se depende de burós de crédito privados o proveedores de Open Banking que actúan como cuellos de botella costosos y concentran datos sensibles.
3. **Urgencia real y contemporánea:** Con la proliferación de herramientas de IA generativa, la alteración de extractos bancarios y documentos PDF se ha vuelto trivial, haciendo inviables los métodos tradicionales de validación manual.

### Propuestas descartadas

> Cada propuesta considerada, quién la propuso y el motivo del descarte.

Solo se consideró esta propuesta.

### Cómo tomamos la decisión

> Cómo llegó el equipo al acuerdo: votación, consenso tras debate u otro.

Al ser el unico integrante del equipo, no hubo discución, simplemente me pareció el problema más relevante y con mayor potencial de solución.

---

## Problem Brief

### Encabezado

> Nombre del proyecto y una frase que describa el problema. Extensión: breve.

**Proyecto:** Glemo  
**Problema:** Verificación universal e instantánea de solvencia y datos financieros sin intermediarios y preservando la privacidad del usuario frente a la manipulación por IA.

### Equipo y roles

> Integrantes con su usuario de GitHub, rol asumido por cada persona, responsable de las entregas y canal de coordinación interna. Extensión: breve.

- David Zapata (DavidZapataOh) - Desarrollador.

### Problema y evidencia

> Enunciado del problema en una frase, sin mencionar blockchain. Contexto, frecuencia y alcance. Evidencia mínima de que el problema existe: observación directa, experiencia propia, conversaciones o fuentes consultadas, con enlace o cita cuando aplique. Extensión: 150–300 palabras.

La validación de documentos e información financiera es lenta, vulnerable al fraude y a la falsificación por inteligencia artificial, y obliga al usuario a exponer toda su información privada a terceros.

En el sector fintech y bancario, comprobar ingresos, historial de pagos o saldos bancarios es un procedimiento crítico y diario que se ejecuta millones de veces a nivel global durante la apertura de cuentas, la solicitud de créditos o el acceso a rampas de pago (on/off ramps). Sin embargo, este proceso descansa en una infraestructura analógica: el intercambio de archivos PDF o capturas de pantalla. 

Hoy en día, herramientas accesibles de edición digital y modelos multimodales de inteligencia artificial permiten falsificar un extracto bancario, modificar cifras o crear identidades sintéticas en cuestión de segundos, dejando a los filtros tradicionales completamente desarmados. Reportes recientes del sector de identidad digital señalan incrementos superiores al 300% en intentos de fraude documental impulsados por IA generativa en servicios financieros. 

Por otro lado, cuando las entidades intentan mitigar este riesgo recurriendo a proveedores tradicionales de Open Banking o burós centralizados, se encuentran con un ecosistema fragmentado: en mercados emergentes como Latinoamérica, la gran mayoría de instituciones bancarias no disponen de APIs públicas o sus conexiones sufren caídas constantes. Esto obliga a las entidades a mantener extensos equipos de operaciones manuales para cotejar información, mientras que los solicitantes legítimos se ven forzados a entregar extractos completos con historiales exhaustivos de consumo, exponiendo su privacidad financiera a fugas de datos y brechas de seguridad.

### Usuario y actores

> Quién sufre el problema y qué necesita resolver. Cómo lo resuelve hoy y qué le cuesta en dinero, tiempo o esfuerzo. Demás actores que intervienen en el flujo, con el papel que cumple cada uno. Extensión: 150–300 palabras.

El problema afecta directamente a dos actores principales en cada transacción:

1. **El solicitante (persona o empresa):** Necesita demostrar solvencia o titularidad para acceder a un servicio financiero (un préstamo, una rampa fiat-cripto o una cuenta comercial). Actualmente lo resuelve descargando extractos en PDF o compartiendo credenciales bancarias. Este método le cuesta días de espera, fricción burocrática y una pérdida total de soberanía sobre sus datos, ya que entrega transacciones personales detalladas e irrelevantes para la evaluación crediticia.
2. **El oficial de riesgo y cumplimiento (Compliance Officer / Fintech):** Necesita determinar la veracidad de la información financiera recibida para prevenir fraude y cumplir normativas de prevención de lavado de activos (AML) y debida diligencia (KYC). Hoy lo resuelve mediante cotejo manual, llamadas telefónicas o sistemas de OCR que le cuestan entre $5 y $25 dólares por revisión, con tiempos de respuesta de 48 a 72 horas y altas tasas de abandono en el embudo de conversión.

**Demás actores del flujo:**
* **Bancos emisores:** Alojan los fondos y emiten los extractos. Operan como silos cerrados que no tienen incentivos comerciales para crear APIs de consulta gratuitas para terceros competidores.
* **Burós de crédito y agregadores de datos:** Cobran tarifas recurrentes elevadas por bases de datos que suelen estar desactualizadas y concentran riesgos sistémicos de ciberseguridad.
* **Reguladores financieros:** Exigen estándares rigurosos de verificación de solvencia y auditoría, pero al mismo tiempo imponen sanciones severas ante la filtración de datos sensibles de los usuarios.

### Flujo actual de valor

> Recorrido paso a paso de cómo se mueve hoy el dinero, la información o el activo, desde el origen hasta el destino. Diagrama o secuencia numerada, con los intermediarios explícitos. Señalar si algún paso responde a una obligación normativa. Extensión: 150–300 palabras.

El recorrido habitual de la información financiera desde su origen hasta la aprobación sigue una secuencia lineal altamente fragmentada:

1. **Solicitud de servicio:** El usuario ingresa a la plataforma fintech o entidad financiera y solicita un producto (por ejemplo, una línea de crédito o un desembolso fiat).
2. **Requerimiento documental:** El sistema de la entidad exige al solicitante comprobantes de ingresos y extractos bancarios recientes para satisfacer exigencias normativas de debida diligencia (KYC/AML).
3. **Extracción por el usuario:** El usuario inicia sesión en la web de su banco tradicional, descarga su extracto bancario en formato PDF o realiza capturas de pantalla de sus movimientos.
4. **Carga y transferencia:** El solicitante sube el archivo PDF sin cifrar a través del portal de la fintech o lo remite por correo electrónico.
5. **Revisión por intermediarios y OCR:** La entidad procesa el documento mediante un software centralizado de OCR (reconocimiento óptico de caracteres) para digitalizar las cifras y envía el caso a una cola de revisión humana.
6. **Validación externa (opcional):** La entidad intenta cruzar el número de identificación con burós de crédito privados pagando una tarifa por consulta. Si la información no coincide o el documento parece sospechoso, un analista llama manualmente a la sucursal o solicita documentación complementaria.
7. **Resolución y dictamen:** Tras un lapso de 1 a 4 días hábiles, el analista aprueba o rechaza manualmente la solicitud y archiva los documentos completos en bases de datos internas de la compañía.

### Fricciones identificadas

> Puntos concretos donde el flujo falla, se encarece o se demora. Cada fricción indica en qué paso ocurre, qué la causa y a quién afecta. Extensión: 150–300 palabras.

**Fricción 1: Vulnerabilidad absoluta a la falsificación por IA (Paso 3 y 4)**  
  *Causa:* Los documentos PDF y las imágenes no poseen firmas criptográficas vinculadas al origen; cualquier editor de texto o modelo generativo puede alterar saldos y fechas sin dejar huellas visibles.  
  *Impacto:* Afecta a la entidad receptora, exponiéndola a pérdidas por fraude crediticio y carteras vencidas irrecuperables.
* **Fricción 2: Demoras extremas y altos costos operativos (Paso 5 y 6)**  
  *Causa:* La necesidad de intervención humana para desconfiar y verificar datos manualmente en procesos que deberían ser automatizados.  
  *Impacto:* Afecta tanto a la fintech (que asume costos salariales de compliance y licencias de software) como al usuario (que sufre tiempos de espera de hasta 96 horas).
* **Fricción 3: Fuga de privacidad y acumulación de pasivos de datos (Paso 4 y 7)**  
  *Causa:* La arquitectura tradicional de "todo o nada", donde para probar un balance promedio de \$2,000 se debe exponer cada consumo individual, ubicación de compras y datos familiares.  
  *Impacto:* Afecta al usuario, que ve vulnerada su privacidad, y a la empresa, que crea un repositorio centralizado (*honeypot*) susceptible a hackeos y penalizaciones por leyes de protección de datos personales.
* **Fricción 4: Dependencia de silos bancarios y APIs cerradas (Paso 6)**  
  *Causa:* Los bancos comerciales protegen su información y no ofrecen canales de interoperabilidad abiertos ni estables para fintechs emergentes.  
  *Impacto:* Afecta la escalabilidad de las fintechs, limitando su expansión geográfica en mercados emergentes.

### Oportunidad e hipótesis

> Oportunidad priorizada entre las fricciones identificadas, con el motivo de la elección. Hipótesis inicial de por qué blockchain podría mejorar ese punto, expresada en términos de qué cambiaría para el usuario. Extensión: 150–300 palabras.

**Oportunidad priorizada:**  
Eliminar por completo el intercambio manual de documentos y la dependencia de APIs bancarias centralizadas, transformando la verificación de datos en un proceso matemático instantáneo y privado originado directamente desde la sesión web del usuario.

**Hipótesis:**  
Si reemplazamos la carga manual de PDFs por atestaciones criptográficas generadas directamente desde la sesión web autenticada del usuario y las registramos en una red descentralizada mediante pruebas de conocimiento cero (ZK), entonces:
* El tiempo de verificación de solvencia se reducirá de varios días hábiles a **menos de 5 segundos**.
* El riesgo de fraude por adulteración con IA se eliminará por completo, ya que la validez del dato estará matemáticamente respaldada por el servidor emisor.
* La privacidad del usuario se preservará al 100%, ya que el solicitante podrá demostrar que cumple una regla de negocio (ejemplo: *"mis ingresos mensuales superan \$3,000"*) sin necesidad de revelar su saldo total, su identidad completa ni su lista de transacciones.
* Las fintechs y entidades financieras reducirán sus costos operativos de compliance en más del **80%**, acelerando drásticamente sus tasas de conversión.

### Criterio de pertinencia

> Justificación de por qué el caso requiere un registro distribuido y no una base de datos tradicional o una integración entre sistemas existentes. Debe apoyarse en al menos uno de los criterios de la Sesión 1: varias partes que no confían entre sí necesitan compartir un mismo registro, el histórico no puede alterarse, o se elimina un intermediario que hoy concentra la confianza. Extensión: 150–300 palabras.

Este problema no puede resolverse de forma eficiente mediante una base de datos centralizada tradicional o una integración típica entre sistemas por tres razones fundamentales alineadas con la Sesión 1:

1. **Partes que no confían entre sí necesitan compartir un registro único:**  
   El solicitante, la fintech evaluadora y el banco emisor operan en un entorno sin confianza mutua. Una base de datos centralizada administrada por la fintech permitiría que esta altere las condiciones o registros a conveniencia. A su vez, una base de datos administrada por un buró privado recrea un monopolio de información que extrae rentas y excluye a nuevos participantes del sistema financiero.
2. **Eliminación del intermediario que concentra la confianza:**  
   Las soluciones existentes obligan a confiar ciegamente en agregadores externos o burós centralizados que actúan como custodios de la verdad. Una red distribuida permite que la atestación sea autosuficiente y verificable por cualquier entidad mediante matemáticas, prescindiendo de intermediarios centralizados que puedan censurar el acceso o manipular los registros.
3. **Histórico inalterable y auditable para cumplimiento normativo:**  
   Los reguladores financieros exigen que cualquier decisión crediticia cuente con un respaldo de auditoría permanente. En una base de datos relacional ordinaria, los registros pueden ser modificados o purgados por administradores con privilegios elevados. Un registro distribuido garantiza un historial inalterable en el tiempo, demostrando ante cualquier auditoría que la condición financiera se cumplió legítimamente al momento exacto de la aprobación sin necesidad de almacenar los datos privados de los usuarios.

### Supuestos y riesgos

> Dos o tres supuestos que tendrían que ser ciertos para que la hipótesis funcione, y qué podría invalidarla. Extensión: 150–300 palabras.

**Supuestos críticos para el éxito de la hipótesis:**
1. **Acceso web del usuario:** Se asume que el usuario final tiene acceso a su portal bancario o plataforma de origen mediante credenciales web activas y está dispuesto a iniciar sesión a través de una interfaz de verificación criptográfica (extensión o SDK web).
2. **Aceptación regulatoria de atestaciones criptográficas:** Se asume que las entidades de control financiero aceptarán como prueba válida de debida diligencia (KYC/AML) una atestación matemática verificada en un registro distribuido, en lugar de exigir obligatoriamente una copia física o digitalizada del documento original en papel o PDF.
3. **Rendimiento e inmutabilidad de la red:** Se asume que la infraestructura descentralizada seleccionada mantendrá costos por transacción predecibles (fracciones de centavo) y tiempos de confirmación casi instantáneos (menos de 5 segundos) para no perjudicar la experiencia del usuario en el punto de registro.

**Riesgos que podrían invalidar la hipótesis:**
* **Cambios agresivos en la arquitectura web de los emisores:** Si las entidades bancarias implementan contramedidas activas para fragmentar o bloquear las conexiones TLS durante la generación de pruebas off-chain, la tasa de éxito de las verificaciones podría degradarse.
* **Rigidez normativa extrema:** Si la regulación bancaria local insiste taxativamente en que el oficial de cumplimiento debe almacenar el archivo visual del documento bancario con fines probatorios legales, la adopción institucional del modelo de conocimiento cero requerirá cambios legislativos previos.