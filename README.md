# Percepción de la gestión institucional preventiva (PGIP)

Trabajo del curso Diseño y Análisis de Encuestas (Ingeniería Estadística, Universidad de
Santiago de Chile, 2026). Construimos y validamos una escala de seis ítems sobre cómo los
apoderados perciben la prevención de la violencia en el colegio de sus hijos, con las
respuestas de 171.797 apoderados de estudiantes de II medio del Simce 2024.

[Ver la presentación](https://cpizarrof.github.io/pgip-psicometria/)

## Datos

La base une tres fuentes por el RBD del establecimiento: el cuestionario de apoderados
del Simce, los resultados por establecimiento de la Agencia de Calidad (grupo
socioeconómico, dependencia y ruralidad) y el Directorio Oficial del Mineduc (orientación
religiosa). Las bases no se publican aquí: se descargan o solicitan en los sitios de la
Agencia de Calidad de la Educación y del Mineduc.

## Resultados principales

- Los seis ítems forman un solo factor y la consistencia interna es alta (α ≈ 0,88).
  El modelo mantiene su ajuste por grupo socioeconómico, dependencia, zona y orientación
  religiosa.
- La escala se relaciona con las medidas de prevención y se separa de la victimización
  reportada, lo que reduce la preocupación por un efecto halo.
- Las diferencias entre grupos son estadísticamente significativas, pero muy pequeñas:
  las variables de control explican menos del 0,5 % de la varianza.
- No aparece un gradiente socioeconómico. El grupo medio alto obtiene el puntaje más bajo
  (68,0) y el grupo bajo, 72,2, lo que podría reflejar estándares más exigentes en las
  familias con más recursos.

## Métodos

Análisis de ítems, confiabilidad por Teoría Clásica de los Tests, análisis factorial
confirmatorio con lavaan, invarianza de medida, validez convergente y divergente con
corrección por atenuación y una métrica de 0 a 100.

## Cómo reproducirlo

Se necesita R (4.3 o más reciente) y [Quarto](https://quarto.org/docs/get-started/).

```r
install.packages(c("tidyverse", "knitr", "readxl", "psych",
                   "lavaan", "gt", "showtext", "ragg"))
```

Con las tres bases dentro de `presentacion/`:

```bash
quarto render presentacion/presentacion-pgip.qmd
```

## Autores

Bianca Bruna, Cristian Olate y Carlos Pizarro. Profesor: Esteban Avarca Oviedo.
