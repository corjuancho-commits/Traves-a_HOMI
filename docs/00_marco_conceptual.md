# 00. Marco conceptual y de gobernanza

**Versión:** 0.1  
**Estado:** preliminar  
**Propósito:** definir qué es TravesíaHOMI, qué problema resuelve y qué principios no deben perderse al desarrollar las demás capas.

## 1. Propósito

TravesíaHOMI es un sistema de orquestación de entrenamiento al rol de enfermería orientado a que el personal nuevo transite desde el ingreso institucional hasta una autonomía progresiva y segura. Integra preparación inicial, experiencias de aprendizaje distribuidas, práctica clínica supervisada, seguimiento y trazabilidad.

El sistema no pretende enseñar todas las competencias profesionales de enfermería. Su alcance es más preciso: **identificar y desarrollar las capacidades críticas que HOMI no debería permitir que un colaborador ejerza con autonomía sin haberlas comprendido, practicado o demostrado en el contexto institucional**.

## 2. Problema que busca resolver

El modelo tradicional de inducción tiende a organizarse como una sucesión de capacitaciones dependientes de disponibilidad de líderes y espacios. Esto dificulta:

- conectar contenidos con desempeño real;
- asegurar recuperación y práctica distribuida;
- diferenciar necesidades por rol y servicio;
- manejar grupos de tamaño variable;
- aprovechar simulación con criterio;
- identificar retrasos y necesidades individuales;
- conocer qué experiencias vivió realmente cada participante;
- sostener el aprendizaje durante los turnos de entrenamiento;
- producir datos longitudinales útiles para mejora.

TravesíaHOMI propone sustituir la lógica de “agenda de capacitaciones” por una **trayectoria ejecutable de entrenamiento**.

## 3. Alcance temporal preliminar

La arquitectura se diseña para un continuo compuesto por:

1. **Preparación inicial:** aproximadamente 8–9 días.
2. **Práctica clínica supervisada:** 10 turnos de entrenamiento en servicio.
3. **Autonomía inicial acompañada:** seguimiento hasta aproximadamente el día 30.
4. **Consolidación:** extensión potencial a 60 días o más.

Las duraciones definitivas dependen de los lineamientos institucionales oficiales de entrenamiento al rol.

## 4. Principios

### 4.1 Autonomía estructurada
El participante puede explorar, consultar, practicar, trabajar con pares y gestionar parte de su aprendizaje, pero el sistema define resultados mínimos, dependencias críticas, evidencias y reglas de avance.

### 4.2 Gestión por excepción
El formador no debe perseguir a todos por igual. El sistema debe hacer visible quién avanza normalmente y dónde se requiere intervención humana por retraso, riesgo, reprobación, ausencia de evidencia o dificultad.

### 4.3 Modularidad
La arquitectura del proceso se separa de los contenidos. Los recursos clínicos deben ser pequeños y versionables para que un cambio técnico, científico o normativo no obligue a reconstruir toda la trayectoria.

### 4.4 Aprendizaje longitudinal
Una competencia no se “ve” una vez. Sus nodos pueden aparecer como preparación, práctica, recuperación, aplicación, evaluación y transferencia en distintos momentos.

### 4.5 Intercalado
Los ocho días iniciales no se organizan necesariamente por temas completos. Distintos nodos de varias competencias pueden alternarse y reaparecer de manera espaciada.

### 4.6 Hospital como red de aprendizaje
Los servicios no son cursos. Son ambientes que pueden ofrecer experiencias concretas. Un mismo nodo puede tener varios ambientes posibles y cada ambiente puede tener capacidad, disponibilidad, restricciones y alternativas.

### 4.7 Simulación con justificación
La simulación se asigna por necesidad pedagógica y de seguridad: riesgo, necesidad de repetición, baja predictibilidad clínica, posibilidad de error inicial, necesidad de estandarización o integración.

### 4.8 Decisiones basadas en evidencia de desempeño
Completar una actividad no equivale a demostrar capacidad. El sistema diferencia participación, práctica, demostración, aprobación y transferencia.

### 4.9 Plataforma subordinada al modelo
Buk es una capa tecnológica de implementación. Las definiciones de competencia, nodo, experiencia, evidencia, estado y evento deben mantenerse independientes de la plataforma.

## 5. Gobernanza propuesta

La construcción debe ser colaborativa y gradual. Formación de Enfermería mantiene la arquitectura metodológica; los líderes y expertos clínicos validan competencias, nodos, límites de rol, riesgos y viabilidad operativa; los servicios validan capacidad y condiciones de los ambientes; las capas tecnológica y de datos traducen el modelo sin redefinirlo.

El proyecto debe escalar por fases: una competencia, pocos nodos, piloto, evaluación, ajuste y expansión.

## 6. Regla de control

Ninguna actividad, recurso, curso, simulación o tarea en Buk debería crearse sin poder responder:

1. ¿A qué competencia aporta?
2. ¿Qué nodo desarrolla o evalúa?
3. ¿Qué experiencia representa?
4. ¿Qué evidencia produce?
5. ¿Qué criterio permite interpretar esa evidencia?
6. ¿Qué dato debe conservarse?
