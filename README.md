# Dashboard de restaurante en Power BI

Dashboard de ventas, costes y beneficio de un restaurante, desarrollado en Power BI con limpieza de datos en Power Query. Proyecto realizado durante el Máster en Análisis de Datos para la Gestión Empresarial (UDIMA). Los datos son de práctica.

## Vista previa

![Dashboard](images/1.png)

## Objetivo

Analizar qué categorías de producto generan más ingresos y más beneficio, cómo evolucionan las ventas a lo largo del año y cuáles tienen mejor margen.

## Datos

El archivo Excel tiene dos hojas:
- **RegistroVentas:** registro de ventas con fecha, producto, categoría, subtipo y cantidad (unas 850 filas).
- **PreciosProductos:** catálogo de unos 100 productos con categoría, precio y coste.

## Limpieza de datos (Power Query)

El registro de ventas venía desordenado, con filas sobrantes al principio y los encabezados reales en la fila 5. Pasos principales:
1. Eliminar las filas sobrantes de la parte superior.
2. Promover la fila correcta como encabezados.
3. Corregir tipos de datos (fechas, números y texto).
4. Relacionar las ventas con la tabla de precios y costes por la clave del producto.

## Medidas (DAX)

- **Total ingresos:** suma de precio por cantidad.
- **Total costes:** suma de coste por cantidad.
- **Beneficio:** ingresos menos costes.
- **Margen %:** beneficio dividido entre ingresos.

## Contenido del dashboard

- Gráfico de columnas de ingresos, costes y beneficio por categoría.
- Evolución mensual de ingresos, costes y beneficio.
- Matriz por categoría, con totales y margen.
- Filtros por trimestre.
- Tooltip con un treemap de ingresos por categoría.

## Hallazgos principales

- El restaurante factura unos **46.300 €**, con unos costes de **36.000 €** y un beneficio de **10.300 €**, es decir, un margen cercano al **22 %**.
- **Vinos, Pizzas y Entradas** concentran en torno al **62 % del beneficio**.
- Los **Vinos** tienen el mejor margen (≈31 %), mientras que categorías como Tacos, Fajitas, Sushi Tradicional o Pastas quedan entre el 9 % y el 12 %.
- Las ventas son más altas en **enero** y más bajas en **julio y octubre**.

## Herramientas

Power BI (DAX, Power Query) y Excel.

## Autor

Daniel Fernández Gutiérrez – [LinkedIn](https://www.linkedin.com/in/daniel-fernández-gutiérrez-3a7b542aa)


