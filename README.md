# 📊 Maven Toys — Dashboard de Ventas e Inventario (Power BI)

Dashboard ejecutivo desarrollado en Power BI para Maven Toys, una cadena de 50 tiendas de juguetes en México. El análisis cubre el período enero 2022 – septiembre 2023, con un total de 829,262 transacciones de venta.

## 🎯 Objetivo del proyecto
Responder preguntas clave del negocio:
- ¿Cuáles son las ventas totales, utilidad y margen del negocio?
- ¿Qué tiendas, ciudades y productos tienen mejor desempeño?
- ¿Qué categorías concentran mayor venta y rentabilidad?
- ¿Qué productos y tiendas presentan riesgo de quiebre de stock?

## 🧩 Modelo de datos
Se implementó un *modelo estrella* (Star Schema) con sales como tabla de hechos central y products, stores, inventory y calendar como dimensiones. Se eligió sobre el copo de nieve por su mejor rendimiento con grandes volúmenes de datos (829K+ filas).

## 📐 Medidas DAX destacadas
- *Ventas Totales, **Costo Total, **Utilidad, **Margen %*
- *Ticket Promedio*
- *Riesgo Quiebre*: ratio de unidades vendidas vs. stock disponible — identifica productos con alta urgencia de reposición

## 📈 Estructura del dashboard
- *Página 1 – Resumen Ejecutivo:* KPIs, evolución de ventas, top productos/tiendas, ventas por categoría
- *Página 2 – Inventario y Productos:* ranking de productos, riesgo de quiebre por producto y tienda, stock crítico
- *Página 3 – Hallazgos y Conclusiones*

## 🔑 Hallazgos clave
- *Lego Bricks* lidera en ventas ($2.38M) pero tiene el margen más bajo del Top 10 (12.5%)
- *Colorbuds* es el producto más rentable (53.4% margen) con ratio de riesgo de quiebre de 90
- *Action Figure* presenta el mayor riesgo de quiebre (ratio 94) — prioridad crítica de reposición
- La categoría *Toys* concentra el 35% de las ventas totales ($5.09M)
- El inventario actual ($410,200) representa solo el 2.8% de las ventas totales — señal de alta rotación de stock

## 🛠️ Herramientas utilizadas
Power BI · Power Query · DAX · Modelado de datos (Star Schema)

## 📁 Archivos
- Maven_Toys_Danny.pbix — archivo de Power BI
- Informe_Maven_Toys_Danny.docx — informe técnico completo
