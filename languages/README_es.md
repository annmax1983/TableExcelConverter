# TableGrab

[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión ligera para el navegador que extrae tablas HTML nativas y cuadrículas de datos ARIA/div de cualquier página web, y las exporta como archivos CSV o Excel (XLSX) con un solo clic.

> Basada en Chromium · Manifest V3 · Permisos mínimos · Privacidad ante todo

---

## ¿Por qué TableGrab?

¿Alguna vez has intentado copiar una tabla de un sitio web gubernamental o una plataforma de datos y te has encontrado con un formato desordenado? TableGrab lee directamente la estructura de la tabla y exporta datos CSV o XLSX limpios — sin errores de copiar-pegar, sin pérdida de formato.

| Ventaja | Detalle |
|---------|--------|
| 📊 **Detección automática** | Escanea todas las tablas nativas y cuadrículas ARIA/div (role=grid/treegrid/table) de la página, muestra filas × columnas |
| 📗 **Exportación a Excel** | Celdas combinadas reales, encabezados con estilo/congelados, anchos automáticos, una hoja por tabla |
| 🔗 **Celdas combinadas** | Gestiona correctamente rowspan/colspan, preservando la estructura de la tabla |
| 🧱 **Cuadrículas div** | Lee cuadrículas tipo MUI DataGrid / AG Grid y unifica las columnas fijas duplicadas |
| 👁️ **Vista previa y columnas** | Revisa la tabla antes de exportar y desmarca las columnas que no necesites |
| 📋 **Copiar como TSV / Markdown** | Pega directamente en Excel, Notion, GitHub o aplicaciones de chat |
| 📦 **Exportación por lotes** | Exporta una tabla individual, las seleccionadas o todas a la vez |
| 🔤 **Sin caracteres extraños** | La codificación UTF-8 BOM corrige los problemas con caracteres chinos/CJK |
| ⚡ **Un clic** | Descarga instantánea, sin necesidad de recargar la página |
| 🔒 **Privado** | Permisos mínimos, los datos de las tablas nunca se suben |

---

## Funcionalidades

### 🆓 Gratis

| Funcionalidad | Descripción |
|---------|-------------|
| 📊 **Detección automática de tablas** | Encuentra tablas nativas y cuadrículas ARIA/div válidas, filtra las tablas ocultas/de maquetación |
| 📗 **Exportación XLSX** | Libro con varias hojas, celdas combinadas reales, encabezado congelado, anchos automáticos |
| 🔗 **Soporte de celdas combinadas** | Analiza rowspan/colspan, reconstruye la cuadrícula correctamente |
| 🧱 **Cuadrículas ARIA / div** | Lee estructuras role=grid/treegrid/table (incl. MUI y AG Grid) y unifica las columnas fijas duplicadas |
| 👁️ **Vista previa antes de exportar** | Vista previa desplazable (hasta 50 filas) con casillas por columna |
| ☑️ **Selección de columnas** | Exporta solo las columnas elegidas; la selección se recuerda por tabla |
| 📋 **Copiar TSV / Markdown** | Copia con un clic para Excel, Notion, GitHub o chat, respetando el ajuste de espacios |
| ✅ **Selección múltiple** | Marca varias tablas y exporta las seleccionadas juntas |
| 📦 **Exportación por lotes** | Exporta con un clic todas las tablas de la página |
| 🔤 **UTF-8 BOM** | Corrección de codificación activada por defecto para caracteres chinos/CJK |
| 🧹 **Limpieza de espacios** | Elimina saltos de línea extra, espacios y fragmentos HTML de las celdas |
| 💧 **Resaltado de tablas** | Pasa el ratón sobre la lista de tablas para resaltar la tabla correspondiente en la página |
| 📁 **Nomenclatura inteligente** | Genera automáticamente el nombre del archivo: TituloPagina_tables_marcatiempo.csv / .xlsx |
| 🔒 **Hasta 5 tablas/página** | El nivel gratuito exporta las primeras 5 tablas detectadas en cada página |

### ⭐ Premium (Licencia)

| Funcionalidad | Descripción |
|---------|-------------|
| 📦 **Exportaciones ilimitadas** | Sin límite de 5 tablas — exporta todas las tablas de cualquier página |
| 🔄 **Todas las funcionalidades gratuitas** | Todo lo anterior, sin restricciones |

---

## Vista previa

<p align="center">
  <img src="../icons/icon128.png" alt="Icono de TableGrab" width="80">
</p>

---

## Navegadores compatibles

| Navegador | Estado |
|---------|--------|
| Google Chrome | ✅ Totalmente compatible |
| Microsoft Edge | ✅ Totalmente compatible |

---

## Instalación

| Tienda | Enlace |
|---|---|
| Chrome Web Store | [Instalar en Chrome](https://chromewebstore.google.com/detail/mekelpcokmdjgoiikpedhojmjappfeji) |
| Complementos de Microsoft Edge | [Instalar en Edge](https://microsoftedge.microsoft.com/addons/detail/lhoelnklgfdihllglpjkpbinfkejceah) |

> Instale solo desde las tiendas oficiales de arriba; evite sitios de descarga de terceros.

---

## Uso

1. Visita cualquier página con tablas o cuadrículas de datos ARIA/div
2. Haz clic en el icono de **TableGrab**
3. Las tablas se detectan automáticamente y se listan con información de filas × columnas
4. Pasa el ratón para resaltar, marca para seleccionar; usa **Vista previa** para elegir columnas
5. Haz clic en **Exportar todo**, **Exportar seleccionadas** o **Copiar como TSV / Markdown**
6. El archivo CSV o XLSX se descarga automáticamente

---

## Limitaciones conocidas

- Las cuadrículas div son compatibles cuando exponen roles ARIA (`grid`/`treegrid`/`table` con roles de fila/celda), como MUI DataGrid y AG Grid. Las cuadrículas en Canvas o sin estructura accesible de filas/celdas no se pueden leer
- Las tablas con paginación o desplazamiento virtual solo exportan las filas y columnas presentes en el DOM
- No se puede acceder a tablas en iframes de otro origen (restricción de seguridad del navegador)
- Las tablas dinámicas complejas o cifradas pueden no analizarse correctamente
- Las celdas de más de 32.767 caracteres se truncan para respetar el límite de Excel

---

## Precios

El plan gratuito exporta hasta 5 tablas por página. Una licencia de herramienta individual elimina ese límite de exportación y la suite completa cubre las funciones premium de todas las extensiones VKT.

Consulta [VKT Pricing](https://www.annmax1983.com/pricing.html) para las opciones de licencia y los precios.

## Privacidad

- ✅ Los datos de las tablas o el contenido de la página nunca se suben — el análisis y la exportación CSV/XLSX ocurren localmente
- ✅ Sin analíticas, sin rastreo
- ✅ Permisos: `activeTab` + `scripting` + `downloads` + `storage`, más acceso de host al servidor de licencias oficial
- ✅ `storage` se usa solo para la clave de licencia y la configuración — sin datos de navegación
- 🔑 La activación/validación de la licencia Premium se conecta únicamente al servidor de licencias oficial (api.annmax1983.com) — nunca se transmiten datos de tablas

---

## Aviso de derechos de autor

Esta extensión solo lee las estructuras de tablas ya cargadas en las páginas web y las convierte a formato CSV o XLSX para descarga local. Todos los datos de las tablas y el contenido de las páginas web pertenecen al sitio web original. Los usuarios no deberían utilizar los datos exportados para reproducción comercial, redistribución no autorizada u otros comportamientos que infrinjan los derechos de autor. Toda responsabilidad legal derivada del uso indebido recaerá exclusivamente sobre el usuario.

---

## ❤️ Apoyo

**[👉 Ko-fi — Invítame a un café](https://ko-fi.com/annmax?ref=tablegrab)**
