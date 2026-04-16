# Diagrama de Gantt — Cronograma del Proyecto

```mermaid
gantt
    title Cronograma del Proyecto
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m/%Y
    tickInterval 1month

    section Fase 1: Análisis y Diseño
        Análisis de requisitos y relevamiento                     :a1, 2026-05-04, 2026-05-15
        Diseño del sistema y arquitectura técnica                 :a2, after a1, 2026-05-29
        Diseño de la interfaz de usuario accesible                :a3, after a2, 2026-06-19

    section Fase 2: Desarrollo
        Catálogo de ejercicios con descripciones propioceptivas   :a4, after a3, 2026-07-31
        Motor de personalización basado en reglas                 :a5, after a4, 2026-10-09
        Revisión del motor con profesionales de salud             :a8, after a5, 2026-10-23
        Interfaz y funcionalidades de la aplicación               :a6, after a5, 2026-11-20

    section Fase 3: Pruebas y Validación
        Integración y pruebas funcionales internas                :a7, after a6, 2026-12-18
        Validación con usuarios externos con discapacidad visual  :a9, after a7 a8, 2027-02-07

    section Fase 4: Cierre
        Ajustes posteriores a la validación                       :a10, after a9, 2027-02-21
        Documentación final y preparación de entrega              :a11, after a10, 2027-03-26
```

*Nota.* Las barras muestran las dependencias entre actividades. La revisión con profesionales de salud (a8) depende únicamente del motor de reglas (a5) y puede ejecutarse en paralelo con el desarrollo de la interfaz (a6); ambas son independientes entre sí. La validación con usuarios (a9) requiere que tanto las pruebas internas (a7) como la revisión profesional (a8) estén completadas. El cronograma puede estar sujeto a ajustes según el avance real del proyecto.
