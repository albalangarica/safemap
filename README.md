# Granada SafeMap · prototipo inicial

Prototipo mínimo de la web pública de **Granada SafeMap**.

La idea de esta primera versión es comprobar tres cosas antes de construir nada más:

1. Que GitHub Pages publica correctamente la web.
2. Que el mapa de Granada carga bien en móvil y ordenador.
3. Que tenemos una base visual sencilla sobre la que añadir después locales, fichas, valoraciones y zonas.

## Tecnología

Esta versión usa únicamente:

- HTML
- CSS
- JavaScript
- Leaflet
- OpenStreetMap
- GitHub Pages

No necesita servidor, instalación local, npm ni compilación.

Más adelante, cuando empecemos a guardar valoraciones y comentarios, podremos conectar **Supabase**.

## Estructura inicial

```text
/
├── index.html
└── README.md
```

De momento todo está dentro de `index.html` para que sea lo más fácil posible de probar y modificar.

## Qué hace este prototipo

- Muestra una cabecera de Granada SafeMap.
- Carga un mapa interactivo de Granada.
- Permite hacer zoom y desplazarse.
- Incluye una pequeña tarjeta informativa.
- Está preparado para funcionar bien en móvil.
- No muestra todavía índices reales ni valoraciones.

## Qué NO hace todavía

- No carga el catálogo real de locales.
- No calcula el Índice SafeMap.
- No muestra fichas de locales.
- No permite enviar valoraciones.
- No conecta con Supabase.
- No incluye panel de moderación.

Es intencionado: primero comprobamos que la base funciona en GitHub Pages.

## Cómo publicarlo en GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube `index.html` y `README.md` a la raíz del repositorio.
3. En GitHub entra en:

   **Settings → Pages**

4. En **Build and deployment** selecciona:

   **Deploy from a branch**

5. Selecciona:

   - Branch: `main`
   - Folder: `/ (root)`

6. Guarda.

GitHub mostrará la dirección pública de la web al cabo de unos segundos o minutos.

## Siguiente paso

Cuando este prototipo esté publicado y comprobemos que el mapa funciona, el siguiente paso recomendado es:

**Paso 2 · cargar el catálogo real de locales desde un archivo de datos**

La primera ampliación será añadir un archivo `locales.json` y hacer que el mapa pinte automáticamente los locales reales.

Después avanzaremos por este orden:

1. Catálogo de locales.
2. Ficha de local.
3. Estados “con datos / sin datos”.
4. Ranking de zonas.
5. Formulario de valoración.
6. Supabase.
7. Moderación.

## Criterio importante del proyecto

La web debe distinguir siempre entre la **percepción declarada por las personas usuarias** y una afirmación objetiva sobre un local.

Un local sin suficientes valoraciones debe seguir apareciendo en el mapa, pero sin mostrar un índice que no existe.

---

Prototipo inicial · septiembre de 2026
