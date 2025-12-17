# Libreta de Mantenimiento – Centros de recogida de aceituna

App en **un solo archivo HTML** para registrar, buscar y gestionar anotaciones técnicas de mantenimiento por **población/centro**, con **adjuntos (fotos/documentos)** guardados dentro de la propia app.

## Funcionalidades
- Alta de registros con:
  - **POBLACIÓN**, **CENTRO DE TRABAJO**, **UBICACIÓN EN EL CENTRO**
  - **CATEGORÍA** (motor/polea/rodillo…), **REFERENCIA**
  - **MEDIDAS / ESPECIFICACIONES**
  - **ESTADO** y **REPARADO / REPARAR**
  - **FECHA**
  - **HERRAMIENTAS** y **NOTAS**
  - **FOTOS / DOCUMENTOS** (se guardan como Base64)
- Edición y borrado de registros.
- Búsqueda global por texto y filtros por población, centro, categoría, estado y reparado/reparar.
- Ordenación por fecha, última modificación, población, centro y categoría.

## Almacenamiento
- Los registros se guardan en el dispositivo mediante **IndexedDB**.
- Los adjuntos se guardan **incrustados** (Base64) dentro de cada registro.

## Exportar / Importar
Botones disponibles:
- **EXPORTAR JSON**: copia completa (incluye adjuntos).
- **EXPORTAR EXCEL (CSV)**: compatible con Excel (no incluye Base64; exporta resumen de adjuntos).
- **EXPORTAR PORTAPAPELES**: copia en formato pegable en Excel (tabulado/TSV; sin Base64).
- **IMPORTAR**: restaura desde un JSON exportado.  
  Nota: la importación **reemplaza** el contenido actual.

## Uso
1. Abre el archivo `.html` en el navegador (PC o móvil).
2. Rellena el formulario y pulsa **Guardar**.
3. Usa búsqueda/filtros para localizar registros.
4. Haz copias periódicas con **EXPORTAR JSON**.

## Recomendaciones
- Evita adjuntos demasiado grandes (placas/motores: fotos comprimidas si es posible).
- Haz un backup frecuente con **EXPORTAR JSON** para evitar pérdidas por limpieza del navegador o cambio de dispositivo.

## Licencia
Uso interno / personal (ajústalo si vas a distribuirlo).
