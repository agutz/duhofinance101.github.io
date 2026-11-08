# DÚHO · Sitio web oficial

Sitio estático sin compilación, JavaScript ni dependencias obligatorias. Los archivos de `assets/` se reutilizan sin modificar sus originales. Inter se usa si está instalada; en caso contrario se utiliza la tipografía sans-serif del sistema, sin solicitudes a proveedores de fuentes.

## Antes de publicar

Buscar y reemplazar en `index.html`, `privacy.html` y `terms.html`:

- `[CORREO DE CONTACTO PENDIENTE]`: correo real y atendido del responsable. Aparece también en los pies de página. Se puede convertir en un enlace `mailto:` al completarlo.
- `[NOMBRE DEL RESPONSABLE PENDIENTE]`: nombre de la persona o entidad responsable.
- `[FECHA DE VIGENCIA PENDIENTE]`: fecha efectiva de los documentos legales.

Confirmar que la descripción del respaldo y su eliminación coincide con la versión Android que se publicará. No hay credenciales ni configuración OAuth en esta web. Los metadatos Open Graph básicos están incluidos; cuando exista una URL pública definitiva, se pueden añadir `og:url`, canonical y una imagen social con URL absoluta.

## GitHub Pages

1. Subir `index.html`, `privacy.html`, `terms.html`, `styles.css` y la carpeta `assets` a la raíz de la rama que se publicará.
2. En el repositorio, abrir **Settings → Pages**.
3. En **Build and deployment**, seleccionar **Deploy from a branch**, elegir la rama (por ejemplo, `main`) y la carpeta **/(root)**. Guardar.
4. Esperar a que GitHub indique la URL del sitio. Las rutas relativas admiten tanto un dominio propio como `https://USUARIO.github.io/REPOSITORIO/`.
5. Abrir las tres páginas publicadas. En la configuración de la pantalla de consentimiento de Google OAuth, utilizar las URL públicas definitivas de la página principal, `privacy.html` y `terms.html` en sus campos correspondientes. Completar los datos legales antes de enviar la configuración a revisión.

Si este repositorio también contiene Android, publicar únicamente los archivos web y los recursos necesarios, en una carpeta o rama dedicada cuando corresponda; no subir claves, archivos de firma ni secretos.
