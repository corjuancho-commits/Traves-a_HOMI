# TravesíaHOMI

**Estado:** arquitectura base v0.1 — en diseño y validación.

TravesíaHOMI es una propuesta de **orquestación longitudinal del entrenamiento al rol de enfermería en HOMI**. Su objetivo es conectar la preparación inicial, el entrenamiento supervisado en servicio y el seguimiento posterior mediante una arquitectura común de competencias, nodos, experiencias, evidencias, niveles de supervisión, datos y reglas de proceso.

No se diseña como una colección de cursos ni como una reproducción de la formación universitaria. El sistema busca identificar las **capacidades críticas que HOMI necesita garantizar durante la incorporación al rol**, desarrollar esas capacidades mediante experiencias adecuadas al riesgo y al contexto, y acompañar la progresión hacia una autonomía segura.

## Arquitectura documental

1. [Marco conceptual y de gobernanza](docs/00_marco_conceptual.md)
2. [Modelo semántico: competencias y nodos](docs/01_modelo_semantico_competencias_nodos.md)
3. [Modelo de proceso y orquestación](docs/02_modelo_proceso_orquestacion.md)
4. [Arquitectura de datos y trazabilidad](docs/03_arquitectura_datos_trazabilidad.md)
5. [Arquitectura analítica](docs/04_arquitectura_analitica.md)
6. [Arquitectura de simulación](docs/05_arquitectura_simulacion.md)
7. [EPA y progresión de supervisión](docs/06_epa_supervision.md)
8. [Mapeo de ambientes de aprendizaje](docs/07_mapeo_ambientes_aprendizaje.md)
9. [Integración tecnológica con Buk](docs/08_integracion_buk.md)
10. [Roadmap de validación e implementación](docs/09_roadmap_validacion.md)

## Principios de diseño

- **Arquitectura antes que contenido:** primero se define el sistema que mueve el aprendizaje; después se desarrollan los recursos.
- **Autonomía estructurada:** el participante puede autogestionar parte de su experiencia dentro de límites, secuencias y criterios definidos.
- **Gestión por excepción:** la supervisión humana se concentra donde el riesgo, el desempeño o la desviación lo requieren.
- **Modularidad y versionamiento:** competencias, nodos, experiencias, recursos y reglas deben poder evolucionar sin reconstruir toda la ruta.
- **Hospital como red de aprendizaje:** un nodo puede desarrollarse en varios ambientes y un servicio puede ofrecer múltiples oportunidades de aprendizaje.
- **Simulación justificada por nodo:** no se plantea “un día de simulación”; se utiliza cuando la naturaleza, riesgo o predictibilidad de la experiencia lo exige.
- **Datos independientes de la plataforma:** Buk es una capa de implementación; el modelo conceptual, de proceso y de datos debe existir fuera de Buk.
- **Escalamiento progresivo:** se valida competencia por competencia y nodo por nodo antes de ampliar el sistema.

## Horizonte temporal preliminar

La arquitectura se diseña para cubrir, como mínimo:

- preparación inicial de aproximadamente **8–9 días**, pendiente de contraste con lineamientos institucionales definitivos;
- **10 turnos de entrenamiento supervisado**;
- seguimiento inicial alrededor del **día 30**;
- extensión potencial a **60 días o más** según transferencia y necesidades del rol.

## Estado de madurez

Este repositorio contiene documentos técnicos **v0.1**. Las competencias, nodos, tiempos y reglas aquí descritos son hipótesis estructuradas sujetas a validación con lineamientos oficiales, líderes clínicos, expertos de programa, capacidades reales de los servicios y pruebas en Buk.
