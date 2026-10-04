# Gyoza House — Formulario de pedidos

Formulario público (GitHub Pages) para registrar pedidos de Gyoza House que entran
por WhatsApp u otros canales. Calcula el resumen de cocina y financiero, valida
reglas de negocio, y envía cada pedido como una fila nueva a un Google Sheet vía
Apps Script.

Fuente / documentación completa (schema del Sheet, código del Apps Script,
instrucciones de deploy): carpeta `order management/` del proyecto
**Gyoza House OS** (repo privado interno) — este repo es solo la copia pública
desplegable del `index.html`.

## Configurar

Antes de usar en producción, edita `index.html` y reemplaza:

```js
const SHEET_WEBHOOK_URL = 'PASTE_YOUR_APPS_SCRIPT_URL_HERE';
```

con la URL `/exec` de tu Apps Script Web App (ver instrucciones en el repo interno).
