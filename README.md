# 🚗 Análisis de Rentabilidad en un Concesionario de Coches de Ocasión

## Descripción del Proyecto

Este proyecto analiza las operaciones de venta de un concesionario de coches de ocasión con el objetivo de evaluar su rentabilidad, identificar patrones de venta y detectar oportunidades de mejora en la gestión comercial.

Se ha trabajado con un dataset sintético que simula más de 3.000 transacciones realizadas entre 2021 y 2025.

El análisis incluye:
- Limpieza y transformación de datos
- Análisis exploratorio (EDA)
- Cálculo de KPIs clave de negocio
- Evaluación de rentabilidad por marca y modelo

### Estructura del Proyecto
├── data/ # Dataset original en formato CSV
├── analisis/ # Archivo Excel con limpieza y análisis
├── imagenes/ # Gráficos exportados
├── README.md # Documentación del proyecto

###
1. Creación de dataset y análisis
He creado mi propio dataset usando Mockaroo, generando 2.500 filas que simulan las ventas de un concesionario de coches de ocasión. El proyecto se realizará en Google Sheet y voy a importar 3 CSV (me los he tenido que descargar por partes para completar el número de 2500 filas) y anexarlos en una misma hoja. 
2. Transformación y limpieza:
   - En la columna de precio_compra, busco y reemplazo puntos por comas para que Google Sheet lo reconozca como número. En la columa de precio_venta (hasta ahora vacía) incluyo esta fórmula: =K2*(1 + ALEATORIO.ENTRE(30;50)/100) para que me de precios de venta aleatorios.
   - Había puesto ids de ventas pero he decidido cambiarlo por matrículas (3 nuevos exports de Mockaroo)
   - Convierto en tabla y compruebo y si hay duplicados mediante formato condicional (no hay ya que cada coche tiene una matrícula). También he eliminado las filas restantes de debajo de la tabla.
   - En la columna de género, solo quiero que aparezca hombre o mujer así que como está en inglés, voy a reemplazar 'female' por mujer y 'male' por 'hombre', tb hay '
