# Dashboard de Instagram · Plantilla para alumnas

Proyecto educativo basado en el dashboard de Instagram de Vanessa Scott / Emprendedoras Magnéticas. Incluye el asistente de conexión individual y el panel de métricas.

## Instalación sin programar

1. Descarga el ZIP y **descomprímelo** en tu computadora.
2. Abre la carpeta `dashboard-instagram`. No subas el ZIP a GitHub.
3. Dentro verás las carpetas `api`, `css` y `js`, además de los archivos del proyecto. No abras esas carpetas ni saques sus archivos.
4. Crea un repositorio nuevo en GitHub y abre la opción **uploading an existing file**.
5. Desde Finder o el Explorador de archivos, selecciona todo lo que está dentro de `dashboard-instagram` y **arrástralo directamente** al recuadro de GitHub. No uses el selector del navegador para escoger los archivos uno por uno.
6. Antes de confirmar, comprueba que GitHub muestre rutas como `api/analyze.js`, `css/style.css` y `js/wizard.js`. Si muestra `analyze.js`, `style.css` y `wizard.js` sueltos, cancela: la estructura se perdió.
7. Presiona **Commit changes**.
8. En Vercel, elige **Add New > Project > Import Git Repository**, selecciona tu repositorio y despliega usando la configuración predeterminada: sin framework y con el directorio raíz vacío.
9. Espera hasta que el deployment indique **Ready** y abre el enlace HTTPS.
10. Sigue el asistente para conectar tu token personal de Instagram.

Las skills para crear el reporte mensual y el plan de acción se descargan e instalan en Claude por separado. No forman parte de esta carpeta y no deben subirse a GitHub ni a Vercel.

**No pegues tu token en GitHub, ni en capturas, mensajes o variables públicas de Vercel.** El token se introduce exclusivamente en el asistente del dashboard. No configures `INSTAGRAM_TOKEN` ni `INSTAGRAM_USER_ID` en Vercel.

## Requisitos

- GitHub y Vercel; cuentas propias.
- Instagram profesional y permisos de API autorizados por Meta.
- Token personal vigente y conexión HTTPS.
- La API puede limitar métricas, periodos y datos de audiencia.

## Opcionales y límites

- Análisis con IA: solo si la alumna configura su propia clave `ANTHROPIC_API_KEY` **en el servidor de Vercel**; puede generar cargos por uso.
- Esta plantilla guarda el token y el historial únicamente en el navegador local. Usa un navegador/dispositivo propio y evita computadoras compartidas. Si borras los datos del sitio, también se borra la conexión y el historial local.
- El token se envía por HTTPS a la función del propio despliegue y de allí a la API de Meta. No se coloca en los parámetros URL del navegador.
- La configuración de permisos y pantallas de Meta puede cambiar, por lo que los pasos de generación del token deben confirmarse en la documentación oficial.
- No se ha realizado una prueba de integración en una cuenta nueva de Meta desde esta plantilla.

## Métricas de engagement

- **Perfil (por alcance):** interacciones totales / cuentas alcanzadas × 100.
- **Publicaciones:** promedio de la tasa de cada publicación con alcance disponible; posts sin alcance no entran en ese promedio.
- No compares estas tasas como si midieran exactamente lo mismo.

## Si ves el dashboard en blanco

- Abre tu repositorio y comprueba que existan las carpetas `api`, `css` y `js`.
- Confirma que `wizard.js` esté dentro de `js`, `style.css` dentro de `css` y `analyze.js` dentro de `api`. Si todos aparecen sueltos en la raíz, vuelve a cargar la plantilla arrastrando las carpetas completas desde tu computadora.
- Revisa el despliegue en Vercel y abre su URL HTTPS, no `file://`.
- Si el token caducó, genera otro y vuelve a conectar.
- Haz una actualización completa de la página. Si la app instalable guarda una versión antigua, elimina su caché.

## Créditos

Adaptación de Vanessa Scott para Emprendedoras Magnéticas, basada en el Instagram Dashboard del Clube Divos da IA. Conserva la licencia del repositorio original.
