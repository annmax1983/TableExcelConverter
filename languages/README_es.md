# TableGrab

[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión ligera para el navegador que extrae tablas HTML de cualquier página web y las exporta como archivos CSV con un solo clic.

> Basada en Chromium · Manifest V3 · Permisos mínimos · Privacidad ante todo

---

## ¿Por qué TableGrab?

¿Alguna vez has intentado copiar una tabla de un sitio web gubernamental o una plataforma de datos y te has encontrado con un formato desordenado? TableGrab lee directamente la estructura HTML de la tabla y exporta datos CSV limpios — sin errores de copiar-pegar, sin pérdida de formato.

| Ventaja | Detalle |
|---------|--------|
| 📊 **Detección automática** | Escanea todas las tablas HTML de la página, muestra el conteo de filas × columnas |
| 🔗 **Celdas combinadas** | Gestiona correctamente rowspan/colspan, preservando la estructura de la tabla |
| 📦 **Exportación por lotes** | Exporta una tabla individual, las seleccionadas o todas a la vez |
| 🔤 **Sin caracteres extraños** | La codificación UTF-8 BOM corrige los problemas con caracteres chinos/CJK |
| ⚡ **Un clic** | Descarga instantánea, sin necesidad de recargar la página |
| 🔒 **Privado** | Permisos mínimos, los datos de las tablas nunca se suben |

---

## Funcionalidades

### 🆓 Gratis

| Funcionalidad | Descripción |
|---------|-------------|
| 📊 **Detección automática de tablas** | Encuentra todas las tablas HTML válidas, filtra las tablas ocultas/de maquetación |
| 🔗 **Soporte de celdas combinadas** | Analiza rowspan/colspan, reconstruye la cuadrícula correctamente |
| 📋 **Exportación individual** | Exporta cualquier tabla como CSV |
| ✅ **Selección múltiple** | Marca varias tablas y exporta las seleccionadas juntas |
| 📦 **Exportación por lotes** | Exporta con un clic todas las tablas de la página |
| 🔤 **UTF-8 BOM** | Corrección de codificación activada por defecto para caracteres chinos/CJK |
| 🧹 **Limpieza de espacios** | Elimina saltos de línea extra, espacios y fragmentos HTML de las celdas |
| 💧 **Resaltado de tablas** | Pasa el ratón sobre la lista de tablas para resaltar la tabla correspondiente en la página |
| 📁 **Nomenclatura inteligente** | Genera automáticamente el nombre del archivo: TituloPagina_tables_marcatiempo.csv |
| 🔒 **Hasta 5 tablas/página** | El nivel gratuito exporta las primeras 5 tablas detectadas en cada página |

### ⭐ Premium (Licencia)

| Funcionalidad | Descripción |
|---------|-------------|
| 📦 **Exportaciones ilimitadas** | Sin límite de 5 tablas — exporta todas las tablas de cualquier página |
| 🔄 **Todas las funcionalidades gratuitas** | Todo lo anterior, sin restricciones |

---

## Vista previa

<p align="center">
  <img src="icons/icon128.png" alt="Icono de TableGrab" width="80">
</p>

---

## Navegadores compatibles

| Navegador | Estado |
|---------|--------|
| Google Chrome | ✅ Totalmente compatible |
| Microsoft Edge | ✅ Totalmente compatible |

---

## Instalación

1. Abre `chrome://extensions/` o `edge://extensions/`
2. Activa el **modo de desarrollador**
3. Haz clic en **Cargar descomprimida** y selecciona la carpeta del proyecto

---

## Uso

1. Visita cualquier página con tablas HTML
2. Haz clic en el icono de **TableGrab**
3. Las tablas se detectan automáticamente y se listan con información de filas × columnas
4. Pasa el ratón para resaltar, marca para seleccionar
5. Haz clic en **Exportar todo** o **Exportar seleccionadas**
6. El archivo CSV se descarga automáticamente

---

## Limitaciones conocidas

- Solo soporta elementos HTML `<table>` — tablas en imágenes, tablas en Canvas y tablas virtuales en JS no son compatibles
- No se puede acceder a tablas en iframes de otro origen (restricción de seguridad del navegador)
- Las tablas dinámicas complejas o cifradas pueden no analizarse correctamente

---

## Precios

| Plan | Precio | Detalles |
|------|-------|--------|
| 🆓 Gratis | $0 | Hasta 5 tablas por página |
| ⭐ Herramienta individual | $2.99/mes o $9.99 de por vida | Exportaciones ilimitadas de TableGrab |
| 🏆 Suite completa | $3.99/mes o $19.99 de por vida | Todas las extensiones VKT premium |

Consulta [VKT Pricing](https://www.annmax1983.com/pricing.html) para más detalles.

## Privacidad

- ✅ Los datos de las tablas o el contenido de la página nunca se suben — el análisis y la exportación CSV ocurren localmente
- ✅ Sin analíticas, sin rastreo
- ✅ Permisos: `activeTab` + `scripting` + `downloads` + `storage`, más acceso de host al servidor de licencias oficial
- ✅ `storage` se usa solo para la clave de licencia y la configuración — sin datos de navegación
- 🔑 La activación/validación de la licencia Premium se conecta únicamente al servidor de licencias oficial (api.annmax1983.com) — nunca se transmiten datos de tablas

---

## Aviso de derechos de autor

Esta extensión solo lee las estructuras de tablas HTML ya cargadas en las páginas web y las convierte a formato CSV para descarga local. Todos los datos de las tablas y el contenido de las páginas web pertenecen al sitio web original. Los usuarios no deberían utilizar los datos exportados para reproducción comercial, redistribución no autorizada u otros comportamientos que infrinjan los derechos de autor. Toda responsabilidad legal derivada del uso indebido recaerá exclusivamente sobre el usuario.

---

## ❤️ Apoyo

**[👉 Ko-fi — Invítame a un café](https://ko-fi.com/annmax?ref=tablegrab)**
