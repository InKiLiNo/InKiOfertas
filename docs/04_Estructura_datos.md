# 04. Estructura de datos

## Principio
Separar datos técnicos estructurados y texto final editable. Los valores por defecto se copian al equipo al crearlo; cambiar una plantilla en el futuro no modifica ofertas existentes.

## Entidades

### Oferta
ID interno, número, revisión, cliente, fecha, proyecto/referencia, descripción, cantidad, fechas de creación/modificación.

### Equipo
ID, oferta asociada, modelo (`KLOPPER_PATAS` o `KLOPPER_CARTELAS`), diámetro interior, altura cilíndrica, espesores de virola/fondo superior/fondo inferior, volúmenes calculados, altura total y versión de las reglas de cálculo.

### Materiales
Grupo en contacto, grupo sin contacto y excepciones justificadas.

### Soportación y elementos estándar
Tipo de soportación; datos básicos de patas o número de cartelas; número de orejetas; presencia de soporte de placa; materiales y escudos intermedios.

### Aislamiento
Activado/desactivado; zonas; material aislante; espesor; tipo y material del revestimiento.

### Acabados
Acabado interior, acabado exterior y rugosidad cuando corresponda.

### Diseño
Presión, temperatura y norma.

### Conexión
Colección de filas: cantidad, DN/diámetro, tipo, norma/especificaciones y longitud de salida si se registra por conexión.

### Accesorio
Colección de filas: cantidad, descripción y observaciones.

### Texto de oferta
ID, oferta/equipo, texto generado, texto editado, fecha y versión de generación.

## Reglas
- Modelo de datos preparado para que una oferta pueda contener varios equipos, aunque la primera interfaz pueda empezar con uno.
- Conexiones y accesorios son listas de filas.
- Las plantillas son versionadas.
- Los cálculos guardan referencia a la versión de fórmula utilizada.
- Los datos manuales no se sobrescriben con resultados calculados.

## Pendientes
Elegir tecnología y almacenamiento; validar fórmulas Klopper; confirmar experiencia de uno o varios equipos por oferta; inspeccionar plantilla Word.
