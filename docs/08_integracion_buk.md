# 08. Integración tecnológica con Buk

**Versión:** 0.1  
**Estado:** hipótesis de implementación; validar en tenant HOMI

## 1. Principio

Buk no define la pedagogía ni la arquitectura de datos. Se utiliza como plataforma de ejecución, seguimiento y automatización donde sus capacidades aporten valor.

## 2. Mapeo funcional preliminar

### HCM
Contexto de persona, cargo, área y otros atributos laborales.

### Onboarding
Tablero macro de la trayectoria y sus hitos visibles para el participante.

### Rutas de aprendizaje
Secuenciación de cursos y prerrequisitos cuando correspondan.

### Cursos e-learning
Experiencias digitales, recursos, evaluaciones y actividades autogestionadas.

### Cursos presenciales
Registro de experiencias físicas: sesiones, talleres, simulación u otras actividades fuera del reproductor.

### Encuestas / BukForms
Captura estructurada de respuestas, evidencias y determinados productos.

### Workflow
Reacción a eventos y gestión de excepciones: aprobación, reprobación, vencimiento, tareas u otras consecuencias.

### Transferencia / desempeño
Posibles mecanismos para seguimiento posterior.

### Knowledge Center
Candidato para publicar conocimiento institucional validado sobre nodos, ambientes o recursos, sujeto a disponibilidad y gobernanza.

## 3. Regla de traducción

Antes de crear cualquier objeto en Buk debe existir la relación:

**Objeto Buk → ID canónico TravesíaHOMI → competencia/nodo → propósito → evidencia → criterio**

Un curso no debe convertirse por accidente en la unidad conceptual del sistema.

## 4. Codificación

La metodología operativa de códigos Buk puede desarrollarse de forma específica, pero debe:

- referenciar IDs canónicos;
- distinguir tipo de objeto;
- evitar dependencia exclusiva del nombre;
- conservar versión;
- permitir agrupación por programa/ruta/competencia/nodo;
- ser comprensible y reproducible.

## 5. Limitaciones de trabajo ya identificadas

Estas condiciones deben verificarse en el tenant y no asumirse como reglas absolutas:

- progreso/completitud y aprobación pueden representar estados distintos;
- la granularidad temporal varía según el tipo de objeto;
- algunas automatizaciones pueden requerir más de una plantilla;
- no todas las evidencias actúan como bloqueo de avance;
- ciertas trazas de IA/tutor pueden no ser exportables;
- las integraciones externas pueden requerir API o configuración adicional.

## 6. Datos

Buk debe considerarse una fuente operativa. Los identificadores propios de Buk deben mapearse a IDs canónicos. Cuando una señal importante no pueda capturarse en Buk, la arquitectura debe permitir otra fuente sin romper el modelo.

## 7. Validación tecnológica

Antes de escalar TravesíaHOMI deben probarse en el tenant, al menos:

- semántica real de prerrequisitos;
- comportamiento de reprobación;
- múltiples workflows por evento;
- gestión de errores/reintentos;
- evidencias requeridas;
- exportación de datos;
- permisos;
- capacidades disponibles según plan contratado.
