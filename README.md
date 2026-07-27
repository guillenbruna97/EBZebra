# El Marcador

Recap semanal interno de actividad en LinkedIn del equipo Zebra Ventures. Genera pique sano, aprendizaje compartido y motivación para publicar, sin ser una evaluación de desempeño.

## Qué hay en este repo

- `emails/semana-1.html` — plantilla HTML del email semanal, formato GHL (tabla, estilos inline), con avatares personalizados de cada perfil. Úsala como base para cada semana.
- `emails/semana-1-sin-avatares.html` — misma plantilla sin avatares, por si un email necesita salir rápido sin depender de subir imágenes.
- `emails/plantilla-texto-plano.txt` — versión en texto plano, más rápida de producir cuando no hace falta el HTML completo.
- `assets/avatars/` — avatares circulares con anillo de marca (Zebra Yellow `#FFD546`) de los 8 perfiles, listos para subir a la librería de medios de GHL.

## Cómo usar la plantilla HTML cada semana

1. Duplica `emails/semana-1.html` y renómbrala `semana-X.html`.
2. Sube a GHL los avatares de `assets/avatars/` que aún no estén en su librería de medios (solo hace falta una vez, luego se reutilizan).
3. Sustituye los placeholders:
   - `{{URL_AVATAR_MVP}}` por la URL del avatar de quien gane esa semana.
   - `{{URL_AVATAR_1}}` a `{{URL_AVATAR_5}}` por las URLs de los avatares en orden de ranking.
   - `[Nombre]`, `[X.X%]`, `[alcance]`, `[tema del post]` por los datos reales de la semana.
   - `[fecha inicio]–[fecha fin]` por el rango de fechas.
4. Rellena "Qué funcionó" y "Tip para el lunes" con contenido concreto, no genérico.

## Reglas del sistema (no cambiar sin querer)

- **Métrica de ranking:** Engagement Rate — (reacciones + comentarios) / alcance × 100. Nunca alcance bruto, para nivelar perfiles de distinto tamaño de audiencia.
- **Umbral mínimo:** 100 impresiones para entrar al ranking competitivo. Por debajo, el perfil aparece en el bloque "Cogiendo impulso", sin tono negativo ni comparación directa.
- **Tono:** motivador, con algo de pique, sin vergüenza para quien no publicó. Quien no llega al umbral simplemente no aparece en el ranking, no se le señala.
- **Cadencia:** email los viernes. Cada perfil manda su métrica el jueves o viernes.
- **Gamificación:** por ahora solo ranking + MVP. Insignias, rachas e hitos se añaden en fases posteriores — la card de MVP y las filas del ranking ya están preparadas para admitir un badge adicional sin rediseñar el layout.

## Paleta y tipografía (Manual de Identidad 2026)

- Zebra Yellow `#FFD546` · Ink `#1A1A22` · Cream `#FFFCF5` · Yellow Soft `#FFE48A` (fondo de la card MVP) · Plata `#848C99` (texto secundario).
- Red Hat Display (headings) · Red Hat Text (cuerpo).
- Aurora Sun (Cream + Sol) como paleta de esta pieza.

## Nota técnica GHL

Las imágenes van siempre vía URL del CDN de GHL, nunca en base64 incrustado. El editor de GHL respeta tablas con estilos inline; evita flexbox y CSS externo. La importación de Google Fonts va dentro de un `<div>` oculto en el `<body>`, porque GHL elimina el `<head>` del HTML pegado.
