# El Marcador

Recap semanal interno de actividad en LinkedIn del equipo Zebra Ventures. Genera pique sano, aprendizaje compartido y motivación para publicar, sin ser una evaluación de desempeño.

## Qué hay en este repo

- `index.html` — landing del ranking semanal, publicada vía GitHub Pages. Se edita cada semana con los datos nuevos y se sube; la URL es siempre la misma.
- `assets/avatars/` — avatares circulares con anillo de marca (Zebra Yellow `#FFD546`) de los 8 perfiles, referenciados directamente desde `index.html`.

## Cómo actualizar el ranking cada semana

1. Abre `index.html` y sustituye los placeholders:
   - `[Nombre]`, `[X.X%]`, `[alcance]`, `[tema del post]` por los datos reales de la semana.
   - `[fecha inicio]–[fecha fin]` por el rango de fechas.
   - Los `src` de los avatares en la card MVP y en cada fila del ranking, por el archivo correspondiente en `assets/avatars/`.
2. Rellena "Qué funcionó" y "Tip para el lunes" con contenido concreto, no genérico.
3. Haz commit y push a `main`. GitHub Pages redeploya automáticamente en 1-2 minutos.
4. Redacta tú el email o mensaje de Slack avisando de la actualización, con el link a la landing (ver "Publicar en GitHub Pages" más abajo).

## Publicar en GitHub Pages

Si Pages todavía no está activado en este repo:

1. Ve a `Settings` → `Pages` en `github.com/guillenbruna97/EBZebra`.
2. En "Build and deployment", selecciona `Deploy from a branch`.
3. Rama `main`, carpeta `/ (root)`.
4. Guarda. La URL pública queda en `https://guillenbruna97.github.io/EBZebra/`.

## Reglas del sistema (no cambiar sin querer)

- **Métrica de ranking:** Engagement Rate — (reacciones + comentarios) / alcance × 100. Nunca alcance bruto, para nivelar perfiles de distinto tamaño de audiencia.
- **Umbral mínimo:** 100 impresiones para entrar al ranking competitivo. Por debajo, el perfil aparece en el bloque "Cogiendo impulso", sin tono negativo ni comparación directa.
- **Tono:** motivador, con algo de pique, sin vergüenza para quien no publicó. Quien no llega al umbral simplemente no aparece en el ranking, no se le señala.
- **Cadencia:** actualización los viernes. Cada perfil manda su métrica el jueves o viernes.
- **Gamificación:** por ahora solo ranking + MVP. Insignias, rachas e hitos se añaden en fases posteriores — la card de MVP y las filas del ranking ya están preparadas para admitir un badge adicional sin rediseñar el layout.

## Paleta y tipografía (Manual de Identidad 2026)

- Zebra Yellow `#FFD546` · Ink `#1A1A22` · Cream `#FFFCF5` · Yellow Soft `#FFE48A` (fondo de la card MVP) · Plata `#848C99` (texto secundario).
- Red Hat Display (headings) · Red Hat Text (cuerpo).
- Aurora Sun (Cream + Sol) como paleta de esta pieza.
