# Taller FORM-TL-05 — Revisión Técnica Cruzada del Código del PFC

**Universidad Técnica Estatal de Quevedo**
Facultad de Ciencias de la Computación · Carrera de Ingeniería de Software
Asignatura: Aplicaciones Distribuidas (ISR-701)
Unidad 5 — Desarrollo en Capas y Calidad

## Equipo revisor

**Sigla:** BCEL

| Integrante | Rol |
|---|---|
| Castro López Pedro Leonardo | Líder / Editor / Revisión Bloques C, D, E |
| Emanuel Pino Juliana Romina | Revisión Bloques A y B (SOLID y Patrones) |
| Villamarín Cuenca Iván Andrés | Integrante |
| Vinueza Sánchez Harold Nicolás | Integrante |

## Objeto revisado

- **Equipo autor del PFC:** FUVV
- **Sistema:** SCLI — Sistema de Control de Laboratorios e Infraestructura
- **Repositorio revisado:** https://github.com/iavillamarin98-pred/Proyecto_Fin_de_Curso_scli
- **Commit auditado (SHA corto):** `49ec17d`
- **Fecha de auditoría:** 2026-08-11

## Contenido del repositorio

- `informe_revision.tex` — Fuente LaTeX del informe.
- `informe_revision.pdf` — Informe compilado.
- `referencias.bib` — Bibliografía en formato BibTeX (referencia; el informe usa `thebibliography` embebida).
- `README.md` — Este archivo.

## Compilación del informe

### Requisitos

- Distribución TeX completa: **MiKTeX** (Windows) o **TeX Live** (Linux/macOS).
- Paquetes: `inputenc`, `fontenc`, `babel`, `geometry`, `booktabs`, `tabularx`, `array`, `titlesec`, `hyperref`, `graphicx` (MiKTeX los instala automáticamente).
- **No requiere `biber`**: la bibliografía va con `thebibliography` estándar.

### Comandos de compilación

Desde la raíz del repositorio:

```bash
pdflatex -interaction=nonstopmode informe_revision.tex
pdflatex -interaction=nonstopmode informe_revision.tex
```

En PowerShell (Windows), en una sola línea:

```powershell
pdflatex -interaction=nonstopmode informe_revision.tex; pdflatex -interaction=nonstopmode informe_revision.tex
```

Se ejecuta `pdflatex` dos veces para resolver referencias cruzadas de tablas. El resultado es `informe_revision.pdf`.

## Issues abiertos en el repositorio revisado

Los nueve hallazgos verificados fueron reportados como *issues* en el repositorio de FUVV:

https://github.com/iavillamarin98-pred/Proyecto_Fin_de_Curso_scli/issues

Cada *issue* incluye evidencia localizada (archivo y líneas), severidad y bloque del *checklist* de la rúbrica FORM-TL-05.

## Declaración de uso de inteligencia artificial generativa

El equipo revisor BCEL declara haber utilizado un asistente de IA como apoyo para sistematizar la lectura del código auditado, redactar la estructura del informe y verificar el formato IEEE de las referencias. Todos los hallazgos fueron verificados manualmente contra el código del commit `49ec17d`. La responsabilidad intelectual del contenido corresponde a los integrantes del equipo revisor.
