# 03. Arquitectura de datos y trazabilidad

**Versión:** 0.1  
**Estado:** base canónica preliminar  
**Principio:** independiente de Buk

## 1. Objetivo

Definir la estructura mínima de información necesaria para representar TravesíaHOMI, reconstruir trayectorias individuales, soportar analítica, permitir versionamiento y traducir posteriormente el modelo a Buk u otras tecnologías sin perder significado.

## 2. Principio de independencia tecnológica

El modelo canónico no debe depender de nombres de tablas, objetos o restricciones de Buk. La plataforma es una fuente y un motor de ejecución; TravesíaHOMI conserva identificadores y relaciones propias.

## 3. Entidades canónicas

### PERSON
Persona participante.

### WORK_CONTEXT
Contexto laboral relevante: rol, cargo, unidad/servicio previsto, cohorte, fecha de ingreso y condiciones de asignación.

### COMPETENCY
Competencia crítica de inducción.

### NODE
Unidad funcional de una competencia.

### EXPERIENCE
Tipo de experiencia de aprendizaje requerida.

### ACTIVITY
Instancia concreta de una experiencia asignada o realizada.

### ENVIRONMENT
Lugar o contexto: servicio, simulación, Buk, sistema informático, experto, espacio grupal u otro.

### RESOURCE
Objeto utilizado en una experiencia: protocolo, video, caso, equipo, simulador, guía, etc.

### EVIDENCE
Huella observable producida por una actividad.

### ASSESSMENT
Acto o mecanismo de evaluación de una evidencia.

### RESULT
Resultado derivado de la evaluación.

### EPA
Actividad profesional confiable.

### SUPERVISION_LEVEL
Nivel de supervisión/autonomía asociado a una EPA.

### INTERVENTION
Refuerzo, acompañamiento, reentrenamiento, alerta u otra intervención.

### TRANSFER
Evidencia de desempeño posterior en el puesto.

### EVENT
Registro atómico de algo que ocurrió.

### VERSION
Versión vigente de un objeto o definición.

## 4. Relaciones mínimas

- una COMPETENCY contiene muchos NODE;
- un NODE puede requerir varias EXPERIENCE;
- una EXPERIENCE puede implementarse mediante múltiples ACTIVITY;
- una ACTIVITY ocurre en un ENVIRONMENT y puede usar RESOURCE;
- una ACTIVITY puede generar una o varias EVIDENCE;
- una EVIDENCE puede ser interpretada mediante ASSESSMENT;
- ASSESSMENT genera RESULT;
- varios NODE pueden contribuir a una EPA;
- una PERSON puede tener distintos SUPERVISION_LEVEL por EPA;
- un RESULT puede activar una INTERVENTION;
- TRANSFER aporta evidencia longitudinal posterior.

## 5. Granularidad atómica de trazabilidad

La unidad mínima recomendada es un EVENT con estructura conceptual:

**PERSON + OBJECT + ACTION + STATE + TIMESTAMP + CONTEXT + VERSION + SOURCE**

Ejemplo conceptual:

- PERSON: participante X
- OBJECT: C03-N04
- ACTION: práctica_simulada
- STATE: completada
- TIMESTAMP: fecha/hora
- CONTEXT: laboratorio
- VERSION: nodo v1.1
- SOURCE: Buk / formulario / observador / sistema externo

El EVENT no reemplaza la evidencia; registra que algo ocurrió.

## 6. Identificadores

Cada entidad debe tener un identificador canónico estable, único e inmutable. El código no debe depender del nombre visible ni del sistema donde se implemente.

Requisitos:

- unicidad;
- estabilidad temporal;
- no reutilización;
- separación entre ID canónico y nombre visible;
- versionamiento separado del ID;
- posibilidad de asociar uno o varios IDs operacionales de Buk.

La metodología detallada de codificación puede desarrollarse en un proyecto específico, pero debe respetar este contrato.

## 7. Versionamiento

Competencias, nodos, EPA, actividades, recursos y criterios deben versionarse. La trayectoria histórica debe conservar qué versión estaba vigente cuando una persona fue entrenada o evaluada.

Cambiar contenido sin cambiar significado puede ser una revisión menor. Cambiar alcance, criterio, desempeño esperado o relación estructural puede requerir una nueva versión mayor.

## 8. Ruta prescrita y ejecutada

El modelo debe almacenar:

- qué se esperaba que ocurriera;
- qué ocurrió realmente;
- sustituciones de ambientes;
- retrasos;
- reintentos;
- refuerzos;
- cambios de supervisión;
- excepciones.

## 9. Datos mínimos por nodo-persona

Como base analítica, cada relación PERSON–NODE debería poder reconstruir:

- fecha de asignación;
- versión del nodo;
- rol/contexto;
- experiencias requeridas;
- experiencias realizadas;
- ambientes usados;
- evidencias;
- resultados;
- número de intentos;
- necesidad de refuerzo;
- fecha de logro;
- continuidad/transferencia;
- fuentes de datos.

## 10. Calidad de datos

El modelo deberá definir posteriormente reglas de:

- obligatoriedad;
- integridad referencial;
- valores permitidos;
- duplicados;
- consistencia temporal;
- versionamiento;
- trazabilidad de cambios;
- procedencia del dato.

## 11. Privacidad y minimización

La arquitectura debe capturar solo datos necesarios para formación, seguridad, trazabilidad y análisis. La capa analítica debe privilegiar identificadores internos y datos mínimos, evitando replicar información personal innecesaria.

## 12. Relación con Buk

Buk podrá actuar como sistema fuente para contexto laboral, asignaciones, progreso, actividades, evaluaciones y otros eventos. Los IDs de Buk deben almacenarse como claves externas, no reemplazar los IDs canónicos de TravesíaHOMI.
