# Percepción de la Gestión Institucional Preventiva (PGIP)

Propiedades psicométricas y distribución de un constructo de percepción de la gestión
preventiva escolar, medido en **171.797 apoderados** de estudiantes de II Medio
evaluados en el Simce 2024.

**[→ Ver la presentación](https://cpizarrof.github.io/pgip-psicometria/)**

Trabajo de investigación del curso Diseño y Análisis de Encuestas, Ingeniería
Estadística, Universidad de Santiago de Chile.

---

## Qué se hizo

Se construyó y validó una escala de seis ítems que mide cómo los apoderados perciben la
gestión preventiva de la violencia en el establecimiento de sus hijos, y se estudió si
esa percepción difiere entre grupos sociales y territoriales.

La base se ensambló uniendo **tres fuentes** por el Rol Base de Datos (`rbd`): el
cuestionario de apoderados del Simce, los resultados por establecimiento de la Agencia
de Calidad —que aportan grupo socioeconómico, dependencia administrativa y ruralidad— y
el Directorio Oficial del Mineduc, que aporta la orientación religiosa del colegio.

**Ruta psicométrica:** análisis de ítems y descriptivos · confiabilidad por Teoría
Clásica de los Tests · análisis factorial confirmatorio · invarianza por cuatro
variables de control · validez convergente y divergente con corrección por atenuación ·
construcción de la métrica escalar 0–100 · contraste de brechas.

## Resultados

**La escala funciona.** Los seis indicadores convergen en un único factor latente y la
consistencia interna es alta (**α ≈ 0,88**). El modelo mantiene su ajuste al segmentar
por grupo socioeconómico, dependencia, zona geográfica y orientación religiosa: no hay
funcionamiento diferencial por capital cultural.

**Converge y diverge donde debe.** El PGIP se asocia con las medidas de prevención
antiviolencia y se separa de la victimización reportada, sin acoplarse a ella. Eso acota
el efecto halo, que es la objeción natural a una escala de percepción.

**Las brechas existen, pero son irrelevantes.** Las cuatro pruebas resultan
significativas —con 171.797 casos, casi cualquier diferencia lo es—, pero **ningún tamaño
de efecto alcanza siquiera el umbral «pequeño» de Cohen**: las variables de control
explican menos del **0,5 %** de la varianza del constructo.

**Y el patrón no es el esperado.** No hay gradiente socioeconómico. El grupo **Medio
Alto** obtiene el puntaje más bajo de todos (**68,0**), por debajo del GSE **Bajo**
(**72,2**). Es consistente con un sesgo de referencia: más capital cultural, estándares
más exigentes para juzgar al colegio.

La lectura de conjunto es que las familias del país describen una gestión preventiva
notablemente parecida, con independencia de su vulnerabilidad, su territorio, la
dependencia del colegio o su orientación religiosa.

---

## Qué hay en este repositorio

| Carpeta | Contenido |
|---|---|
| `presentacion/` | Código fuente en Quarto + reveal.js, la hoja de estilos y las imágenes |
| `docs/` | La presentación renderizada, que es lo que publica GitHub Pages |
| `data/` | Sólo la documentación de las fuentes: las bases no se republican |

## Cómo reproducirlo

**Requisitos:** R (≥ 4.3) y [Quarto](https://quarto.org/docs/get-started/).

```r
install.packages(c("tidyverse", "knitr", "readxl", "psych",
                   "lavaan", "gt", "showtext", "ragg"))
```

Consigue las tres bases siguiendo `data/README.md`, déjalas dentro de `presentacion/` y
renderiza:

```bash
quarto render presentacion/presentacion-pgip.qmd
```

---

## Autores

Bianca Bruna · Cristian Olate · Carlos Pizarro

Universidad de Santiago de Chile · 2026
