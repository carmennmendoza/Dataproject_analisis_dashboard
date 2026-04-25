# 🚗 Análisis de Rentabilidad en un Concesionario de Coches de Ocasión

## 📖 Descripción del Proyecto

Este proyecto analiza las operaciones de venta de un concesionario de coches de ocasión con el objetivo de evaluar su rentabilidad, identificar patrones de venta y detectar oportunidades de mejora en la gestión comercial.

Se ha trabajado con un dataset sintético que simula más de 3.000 transacciones realizadas entre 2021 y 2025.

El análisis incluye:

- Limpieza y transformación de datos  
- Análisis exploratorio (EDA)  
- Cálculo de KPIs clave de negocio  
- Evaluación de rentabilidad por marca y modelo  

---

## 🗂️ Estructura del Proyecto


├── data/ # Dataset original en formato CSV
├── analisis/ # Archivo en Google Sheets con limpieza y análisis
├── imagenes/ # Gráficos exportados
├── README.md # Documentación del proyecto


---

## 📂 Creación del Dataset

He creado mi propio dataset usando Mockaroo, generando 2.500 filas que simulan las ventas de un concesionario de coches de ocasión.

Debido a las limitaciones de la versión gratuita, descargué varios archivos CSV y posteriormente los uní en una única hoja para trabajar con todos los datos juntos.

El dataset incluye información como clientes, vehículos, precios, márgenes, vendedores y características del coche.

> Nota: Todos los datos son ficticios y se han generado con fines académicos.

---

## 🧹 Transformación y Limpieza de Datos

Durante esta fase se realizaron varias tareas para preparar el dataset:

- Conversión de la columna `precio_compra` a formato numérico (reemplazando puntos por comas).  
- Creación de la columna `precio_venta` mediante la fórmula: =K2*(1 + ALEATORIO.ENTRE(30;50)/100)
- Sustitución del identificador de venta por la matrícula del vehículo para trabajar con un identificador más realista.  
- Comprobación de duplicados mediante formato condicional (no se detectaron duplicados).  
- Eliminación de filas vacías fuera de la tabla.  
- Traducción de valores en la columna de género (`male` → hombre, `female` → mujer, los demás han sido inventados ya que había muchos más géneros y los hemos sutituido al azar).  

---

## 📊 Análisis y Dashboard

El análisis se ha desarrollado en Google Sheets, donde se han creado tablas dinámicas, KPIs y gráficos para visualizar la información.

Se ha construido un dashboard interactivo que permite analizar los datos de forma dinámica mediante controles de filtro.

Durante esta fase surgieron problemas con los filtros, ya que inicialmente estaban configurados sobre tablas dinámicas individuales en lugar de sobre la tabla completa de datos origen. Esto hacía que los filtros no afectasen correctamente a todos los elementos del dashboard.

Para solucionarlo, fue necesario revisar la configuración y aplicar los filtros sobre el rango completo de datos, asegurando que todas las tablas dinámicas estuvieran conectadas correctamente. Para ello, me apoyé en foros y documentación hasta conseguir que el comportamiento fuese el esperado.

---

## 📈 Resultados y Conclusiones

A través del análisis se han identificado diferencias de rentabilidad entre marcas y modelos, así como patrones de venta a lo largo del tiempo.

También se observa cómo variables como el tipo de vehículo o el método de pago pueden influir en el margen obtenido.

Este tipo de análisis permite tomar decisiones más informadas sobre qué vehículos priorizar, cómo optimizar precios y mejorar la estrategia comercial.

---

## 🔄 Próximos Pasos

- Profundizar en el análisis por tipo de cliente  
- Incorporar modelos predictivos de ventas  
- Mejorar el dashboard con mayor interactividad  

---

## 👤 Carmen Mendoza Martos

---

## 🔗 Acceso al archivo

El análisis completo y el dashboard pueden consultarse en el siguiente enlace de Google Sheets:
https://docs.google.com/spreadsheets/d/1Hb3R86NYC1F8dwLlY8NXnKp-jG2_A8i3E0aJvBBrRgg/edit?usp=sharing
