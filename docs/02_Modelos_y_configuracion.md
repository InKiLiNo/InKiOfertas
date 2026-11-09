# 02. Modelos y configuración de depósitos

## Modelos V1
**A. Fondos Klopper y patas**
- Fondos superior e inferior Klopper.
- 4 patas por defecto.
- 2 orejetas de izado por defecto.
- Soporte para placa de características incluido.

**B. Fondos Klopper y cartelas**
- Fondos superior e inferior Klopper.
- 3 cartelas por defecto, según DIN.
- 2 orejetas de izado por defecto.
- Soporte para placa incluido.

En depósitos grandes se pueden poner 3 orejetas; el umbral no está definido y la cantidad será editable.

## Geometría
Campos introducidos:
- Diámetro interior (mm).
- Altura cilíndrica (mm).
- Espesor de virola (mm).
- Espesor de fondo superior (mm).
- Espesor de fondo inferior (mm).

Volúmenes calculados:
- Útil = virola cilíndrica + un fondo Klopper.
- Total = virola cilíndrica + dos fondos Klopper.
Se mostrarán en L y m³. No se descuentan conexiones ni accesorios.

**Pendiente técnico:** validar con THEGSA la geometría y fórmula exacta de los fondos Klopper antes de programar volúmenes y alturas.

Altura total:
- Modelo con patas: suelo hasta punto más alto del fondo superior, incluyendo patas.
- Modelo con cartelas: punto más bajo del fondo inferior hasta punto más alto del fondo superior.
- En patas, distancia vertical nominal entre punto más bajo del fondo inferior y suelo: 500 mm.

**Pendiente técnico:** validar altura exterior de los fondos y cálculo de longitud de patas.

## Redondeo
Resultados calculados redondeados a medidas prácticas, preferentemente múltiplos de 5 o 10 mm. Nunca redondear ni modificar los datos originales introducidos manualmente.

## Patas
- 4 unidades.
- Diámetro de tubo aproximado al 10 % del diámetro del depósito, redondeado a medida comercial.
- Ejemplo: depósito Ø1200 → tubo Ø114,3 (4").
- Separación al suelo: 500 mm desde el punto más bajo del fondo inferior.
- Cantidad, diámetro y longitud editables.
- Si el depósito es 316L: chapa intermedia de refuerzo/escudo 316L (1.4404); tubo de patas 304L (1.4307).

## Cartelas
- 3 unidades, según DIN.
- No calcular dimensiones, peso ni coste en V1.
- Si el depósito es 316L: chapa intermedia de refuerzo/escudo 316L; cartelas 304L.

## Orejetas y placa
- 2 orejetas por defecto; cantidad editable (3 en depósitos grandes cuando proceda).
- Soporte para placa de características siempre incluido inicialmente; editable/eliminable.

## Materiales
Predeterminados:
- En contacto con producto: 316L (1.4404).
- Sin contacto con producto: 304L (1.4307).

Grupo en contacto: virola, ambos fondos y conexiones en contacto con producto.
Grupo sin contacto: soportación y elementos exteriores.
Cambiar materiales por grupos completos, no virola y fondos por separado. Se permiten excepciones justificadas, como escudo intermedio 316L con patas/cartelas 304L. También se podrá configurar equipo completo en 304L o soportación en acero al carbono.

## Aislamiento
- Desactivado por defecto.
- Zonas habituales: cuerpo y fondo inferior; fondo superior sin aislamiento.
- Zonas activables/desactivables individualmente.
- Lana de roca: 40 o 50 mm habitual en pequeños/medianos; 80 mm en grandes. Espesor editable.
- Revestimiento: chapa soldada y estanca; o chapa atornillada de aluminio; o chapa atornillada de inoxidable.
- No automatizar umbral de tamaño para 80 mm en V1.

## Acabados
Predeterminado: decapado + pasivado interior y exterior.
Alternativas seleccionables independientemente:
- Interior pulido espejo Ra < 0,5 µm.
- Exterior satinado Ra < 1,2 µm (Gr. 220).
- Exterior chorreado.

## Diseño
- Presión predeterminada: atmosférica.
- Temperatura predeterminada: ambiente.
- Normas: EN 13445 (habitual para equipos a presión desde 0,5 bar(g)), ASME VIII Div. 1 y AD-2000.
Presión, temperatura y norma editables. La aplicación no sustituye la revisión de aplicabilidad normativa.

## Conexiones
Tabla rápida con orden: cantidad, DN/diámetro, tipo, norma/especificaciones.
Ejemplos:
- 1 Conexión Clamp 1-1/2”, s/ ASME BPE.
- 3 Conexiones DN-50, s/ EN-1092-1 tipo 01 PN10.

Catálogo inicial propuesto (validar al implementar): Clamp, brida, manguito, roscada, DIN, especial/otros. Aproximadamente 5–6 tipos; ampliar catálogo más adelante. Mostrar solo campos pertinentes al tipo.
Longitud de salida habitual 100–150 mm según tamaño; configurable. No afecta a altura total.

## Accesorios
Apartado separado de conexiones. Filas con cantidad, descripción y observaciones opcionales. Ejemplos: bocas de hombre, mirillas, vainas de temperatura, válvulas y otros elementos incluidos. Los elementos estándar del modelo no deben obligar a duplicar su introducción.
