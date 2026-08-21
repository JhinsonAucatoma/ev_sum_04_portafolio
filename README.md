# EV-AUT-03 — Portafolio de Evidencias Individuales

Portafolio individual de Jhinson Stalyn Aucatoma Celorio para la asignatura
Aplicaciones Distribuidas (ISR-701), equipo PFC AGLS — TiendaTech.

## Estructura del repositorio

```
docs/
  informe_portafolio.tex   # Documento principal (LaTeX)
  informe_portafolio.pdf   # PDF ya compilado (incluido para verificación rápida)
  referencias.bib          # Bibliografía (formato IEEE, backend biblatex/biber)
figuras/
  commits-github.png       # Captura del historial de commits del PFC
```

## Requisitos de compilación

- **Distribución:** TeX Live 2023 (o superior) con soporte para `biblatex`
    + `biber`, y los paquetes de idioma español para `babel`.
- **Paquetes del sistema (Ubuntu/Debian):**
  ```bash
  sudo apt-get install texlive-latex-base texlive-latex-recommended \
      texlive-latex-extra texlive-fonts-recommended texlive-bibtex-extra \
      texlive-lang-spanish biber
  ```
- **Archivo principal:** `docs/informe_portafolio.tex`

## Orden de compilación

Desde la carpeta `docs/`:

```bash
pdflatex -interaction=nonstopmode informe_portafolio.tex
biber informe_portafolio
pdflatex -interaction=nonstopmode informe_portafolio.tex
pdflatex -interaction=nonstopmode informe_portafolio.tex
```

El resultado es `docs/informe_portafolio.pdf` (tamaño A4, 6 páginas). Este
mismo PDF ya se incluye compilado en el repositorio para facilitar la
verificación, pero se regenera de forma idéntica siguiendo los pasos
anteriores desde una clonación limpia.

## Verificación

Este documento fue compilado exitosamente desde una clonación limpia del
repositorio siguiendo exactamente los pasos anteriores, sin errores ni
referencias sin resolver.
