# Papillon como app (ícono del cocodrilo + ficha tipo tienda de apps)

Una sola página, un solo ícono. Al abrirla en el navegador muestra una ficha con el logo y el botón OBTENER; ya instalada, al tocar el ícono entra directo a la pantalla de Inicio del sistema.

## 1. Pon la URL de tu app
Abre `config.js` con el Bloc de notas, cambia el texto entre comillas por la URL de la aplicación web (Apps Script -> Implementar -> Administrar implementaciones -> URL de la aplicación web, termina en `/exec`) y guarda. Usa la URL base, sin `?app=`.

## 2. Publícala gratis en GitHub Pages (una sola vez, unos 10 minutos)
1. Crea una cuenta en https://github.com.
2. Botón **New** -> nombre `papillon` -> **Public** -> **Create repository**.
3. **Add file -> Upload files** -> arrastra **todo el contenido** de esta carpeta (index.html, manifest.json, sw.js, config.js y las imágenes) -> **Commit changes**.
4. **Settings -> Pages** -> Branch `main`, carpeta `/ (root)` -> **Save**. En uno o dos minutos queda en `https://TU-USUARIO.github.io/papillon/`.

Esa es la ÚNICA liga que se comparte con todos.

## 3. Instalación en cada equipo
- Android (Chrome): abrir la liga -> **OBTENER** (o menú ⋮ -> Instalar app).
- iPhone/iPad (Safari): Compartir -> **Agregar a inicio**.
- Laptop (Chrome/Edge): **OBTENER** o el ícono de instalar en la barra de direcciones.

## Límites a tener en cuenta
- El sistema sigue corriendo en Google Apps Script. Al abrir desde el ícono, el navegador puede mostrar una barra superior pequeña con la dirección de Google: es una limitación de Google, no se puede quitar.
- Si cambia la URL `/exec`, solo edita `config.js` en GitHub (abrir archivo -> lápiz -> pegar -> Commit). Los íconos instalados siguen funcionando.
- Para un logo más nítido, reemplaza `icon-512.png`, `icon-192.png`, `icon-maskable-512.png` y `apple-touch-icon.png`.
- La página no guarda contraseñas ni datos.
