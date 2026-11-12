# Operaciones de exportación | Indicadores en Power BI

Proyecto académico que reúne indicadores financieros y logísticos para seguir las ventas, la utilidad neta y el cumplimiento de entregas. El tablero analiza **24 meses de finanzas** y **500 pedidos de exportación** del período 2024–2025.

[Ver el tablero en PDF](docs/dashboard_export_operations.pdf) · [Descargar el reporte editable de Power BI](powerbi/dashboard_export_operations.pbix)

## Resultados del período

| Indicador | Cálculo | Resultado |
| --- | --- | ---: |
| Ventas totales | Suma de `Ventas_Totales_CRC` en `Finanzas_Mensual` | **₡982.738.545** |
| Utilidad neta | Suma de `Utilidad_Neta_CRC` en `Finanzas_Mensual` | **₡122.529.508** |
| Margen neto | Utilidad neta total dividida entre ventas totales | **12,47 %** |
| Cumplimiento de entregas | Pedidos marcados como entregados a tiempo y completos, divididos entre el total | **86,20 %** |

De los 500 pedidos, **431** cumplen el criterio de entrega y **69** quedan fuera de él. Las ventas financieras mensuales pasan de ₡27.440.494 en enero de 2024 a ₡53.412.370 en diciembre de 2025.

## Qué muestra el tablero

- Tres tarjetas con medidas DAX de ventas totales, utilidad neta y cumplimiento de entregas.
- Evolución mensual de las ventas financieras y distribución de pedidos según el estado de entrega.
- Montos recibidos por país y producto. Reino Unido lidera por destino con ₡1.583,5 millones y Café Orgánico Certificado lidera por producto con ₡4.421,3 millones.
- Un segmentador de país para explorar los pedidos. La base registra 64 pedidos de Reino Unido, de los cuales 59 cumplen el criterio de entrega, equivalentes al **92,19 %**.

Los indicadores de ventas y utilidad describen las finanzas mensuales de la empresa. El análisis por país y producto utiliza `Monto_Recibido_CRC` de los pedidos de exportación. Cada conjunto conserva su propio alcance y unidad de análisis.

## Datos de origen

| Hoja | Contenido |
| --- | --- |
| `Finanzas_Mensual` | 24 registros mensuales, de enero de 2024 a diciembre de 2025. Fuente de ventas, utilidad y margen. |
| `Pedidos_Exportacion` | 500 pedidos únicos en 10 destinos. Fuente del cumplimiento y los montos recibidos. |
| `Calendario` | 731 fechas de 2024 y 2025 con atributos de año, mes y trimestre. |
| `Marketing_Comercial` y `Produccion_Diaria` | Datos complementarios del caso. |

## Abrir el proyecto

1. Abre `dashboard_export_operations.pbix` en Power BI Desktop.
2. Si Power Query solicita la ubicación del origen, selecciona tu copia local de `export_operations.xlsx` y actualiza el reporte.
3. Explora los pedidos con el segmentador de país. Usa la vista PDF para consultar los resultados generales del caso.

## Archivos del repositorio

| Archivo | Contenido |
| --- | --- |
| [dashboard_export_operations.pbix](powerbi/dashboard_export_operations.pbix) | Reporte editable con medidas, gráficos y segmentador. |
| [dashboard_export_operations.pdf](docs/dashboard_export_operations.pdf) | Vista estática del tablero. |
| [export_operations.xlsx](data/export_operations.xlsx) | Datos de finanzas, pedidos y hojas complementarias. |
| [quiz_export_operations.docx](docs/quiz_export_operations.docx) | Enunciado de la prueba y definiciones de los tres KPIs obligatorios. |

## Autor

**Donald Aguilar Fonseca** · Caso práctico de KPIs y visualización en Power BI.
