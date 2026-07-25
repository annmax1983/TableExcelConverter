# TableGrab
[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión ligera que extrae tablas HTML de cualquier página web y las exporta como CSV con un clic.

> Chromium · Manifest V3 · Permisos mínimos · Local Only

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
| 🔒 **Privado** | Solo3 permisos, sin subida de datos |

---

## Características

- Auto-detección de tablas HTML
- Soporte de celdas combinadas (rowspan/colspan)
- Exportar una, varias o todas las tablas
- UTF-8 BOM para corregir caracteres
- Resaltar tabla al pasar el ratón
- Nombre de archivo automático

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

## Privacidad

- ✅ Sin subida de datos · Sin analíticas · Sin solicitudes de red
- ✅ Solo permisos `activeTab` + `scripting` + `downloads`

---

## Aviso de derechos de autor

Esta extensión solo lee las estructuras de tablas HTML ya cargadas en las páginas web y las convierte a formato CSV para descarga local. Todos los datos de tablas y contenido web pertenecen al sitio web original.

---

## Apoyar

**[👉 Apoyar al desarrollador](https://annmax1983.github.io/TableGrab/)**

---

> **Nota:** Este repositorio es solo para **demostración**. El código fuente completo **no** se publicará aquí.
