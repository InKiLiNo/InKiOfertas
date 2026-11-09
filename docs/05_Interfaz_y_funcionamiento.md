# 05. Interfaz y funcionamiento

## Criterios
Interfaz simple y rápida, basada en modelos preconfigurados. Campos agrupados, valores por defecto visibles y editables. Conexiones y accesorios en tablas con filas añadibles.

## Flujo principal
1. Crear oferta.
2. Introducir número, revisión, cliente, fecha, referencia, descripción y cantidad.
3. Elegir modelo Klopper con patas o con cartelas.
4. Introducir diámetro interior, altura cilíndrica y espesores.
5. Revisar materiales y soportación.
6. Añadir conexiones.
7. Añadir accesorios.
8. Configurar aislamiento si aplica.
9. Seleccionar acabados.
10. Revisar presión, temperatura y norma.
11. Consultar volúmenes y altura calculados.
12. Generar texto técnico.
13. Editar y guardar texto.
14. Exportar Word.

## Pantallas sugeridas
- **Ofertas:** listado, búsqueda, crear, abrir y duplicar ofertas.
- **Datos generales:** número, revisión, cliente, fecha, referencia, descripción y cantidad.
- **Modelo y geometría:** selector de modelos, dimensiones y resumen calculado.
- **Configuración:** materiales/soportación, conexiones, accesorios, aislamiento, acabados y diseño.
- **Texto técnico:** vista previa, edición, guardado y regeneración con aviso.
- **Exportación:** generar Word desde la plantilla THEGSA.

## Comportamientos
- Aplicar valores predeterminados al crear el equipo.
- Si se cambia de modelo, advertir de datos que deban revisarse.
- Permitir añadir, editar, duplicar y eliminar conexiones/accesorios.
- Validar campos y unidades sin imponer límites técnicos no acordados.
- No redondear datos manuales; redondear resultados calculados.
- No perder ediciones manuales del texto.

## Prueba de aceptación V1
Poder crear una oferta, elegir un modelo, introducir geometría, ver cálculos validados, añadir conexiones/accesorios, configurar aislamiento/acabados/diseño, generar y editar texto, y exportar Word conservando la plantilla.

## Para completar exportación
Necesitamos la plantilla Word actual (.docx), una oferta completada representativa y, si existe, un ejemplo de texto técnico especialmente bien redactado.
