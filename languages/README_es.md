# TableGrab
[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión ligera que extrae tablas HTML de cualquier página web y las exporta como CSV con un clic.

> Chromium · Manifest V3 · Permisos mínimos · Privado

---

## ¿Por qué TableGrab?

¿Alguna vez intentaste copiar una tabla de un sitio web y obtuviste un formato desordenado? TableGrab lee la estructura HTML directamente y exporta datos CSV limpios.

| Ventaja | Detalle |
|---------|---------|
| 📊 **Auto-detectar** | Escanea todas las tablas HTML de la página |
| 🔗 **Celdas combinadas** | Soporte rowspan/colspan |
| 📦 **Exportación por lotes** | Una tabla, seleccionadas o todas |
| 🔤 **Sin caracteres** | UTF-8 BOM para caracteres CJK |
| ⚡ **Un clic** | Descarga instantánea |
| 🔒 **Privado** | Permisos mínimos, los datos de tablas nunca se suben |

---

## Características

### 🆓 Gratis

- Auto-detección de tablas HTML
- Soporte de celdas combinadas (rowspan/colspan)
- Exportar una, varias o todas las tablas
- UTF-8 BOM para corregir caracteres
- Resaltar tabla al pasar el ratón
- Nombre de archivo automático
- 🔒 Hasta 5 tablas por página

### ⭐ Premium (Licencia)

- 📦 Exportaciones ilimitadas — sin límite de 5 tablas
- Todas las funciones anteriores, sin restricciones

---

## Vista previa

<p align="center"><img src="icons/icon128.png" alt="TableGrab" width="80"></p>

---

## Instalación

1. Abra `chrome://extensions/` o `edge://extensions/`
2. Active el **Modo desarrollador**
3. Haga clic en **Cargar extensiones desempaquetadas**

---

## Uso

1. Visite cualquier página con tablas HTML
2. Haga clic en el icono de **TableGrab**
3. Las tablas se detectan automáticamente
4. Seleccione y haga clic en **Exportar**

---

## Limitaciones conocidas

- Solo soporta tablas HTML `<table>`
- No soporta tablas de Canvas, imágenes o iframe cruzado

---

## Precios

| Plan | Precio | Contenido |
|------|--------|----------|
| 🆓 Gratis | $0 | Hasta 5 tablas por página |
| ⭐ Herramienta individual | $2,99/mes o $9,99 de por vida | Exportaciones ilimitadas de TableGrab |
| 🏆 Suite completa | $3,99/mes o $19,99 de por vida | Todas las extensiones VKT Premium |

Detalles en [VKT Precios](https://www.annmax1983.com/pricing.html).

## Privacidad

- ✅ Nunca se suben datos de tablas ni contenido de páginas — el análisis y la exportación CSV ocurren localmente
- ✅ Sin analíticas, sin seguimiento
- ✅ Permisos: `activeTab` + `scripting` + `downloads` + `storage`, además de acceso al host del servidor oficial de licencias
- ✅ `storage` solo para licencia y configuración
- 🔑 La activación/validación de la licencia premium solo se conecta al servidor oficial de licencias (api.annmax1983.com) — nunca se transmiten datos de tablas

---

---

## Aviso de código fuente

> ⚠️ **Este repositorio no publica el código fuente.** Contiene únicamente documentación de uso, notas de versión y recursos de soporte. La extensión se distribuye exclusivamente a través de Chrome Web Store. No se proporcionan paquetes de instalación sin conexión ni código fuente para usuarios finales.


## Aviso de derechos de autor

Esta extensión solo lee las estructuras de tablas HTML ya cargadas en las páginas web y las convierte a formato CSV para descarga local. Todos los datos de tablas y contenido web pertenecen al sitio web original.

---

## Apoyar

**[👉 Apoyar al desarrollador](https://annmax1983.github.io/TableGrab/)**

---

> **Nota:** Este repositorio es solo para **demostración**. El código fuente completo **no** se publicará aquí.
