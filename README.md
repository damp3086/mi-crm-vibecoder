# Consola — Mi CRM VibeCoder

Landing page de "Consola", un CRM 2026 para negocios digitales: gestión de clientes, tienda de
productos digitales y captación de leads en redes sociales, todo en una sola página estática
(`index.html`, HTML + CSS + JS inline, sin dependencias de frontend).

## Ejecutar en local

```bash
npm start
```

Levanta un servidor Node mínimo (`server.js`, sin dependencias externas) en `http://localhost:3000`
que sirve `index.html`.

## Desplegar en Railway

1. En Railway, crea un nuevo proyecto y elige **Deploy from GitHub repo**, seleccionando este
   repositorio (`mi-crm-vibecoder`).
2. Railway detecta `package.json` y usa Nixpacks para instalar y ejecutar `npm start`
   automáticamente (configurado también en `railway.json`).
3. No se necesitan variables de entorno: el servidor lee el puerto desde `process.env.PORT`, que
   Railway asigna solo.
4. Al terminar el deploy, Railway expone un dominio público (`*.up.railway.app`) sirviendo la
   página.
