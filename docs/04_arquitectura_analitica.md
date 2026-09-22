# 04. Arquitectura analítica

**Versión:** 0.1  
**Estado:** preliminar

## 1. Objetivo

Definir desde el diseño qué preguntas debe poder responder TravesíaHOMI y qué señales deben capturarse para mejora pedagógica, operativa y de seguridad.

La analítica no se añade al final; determina parte de la granularidad de datos desde el inicio.

## 2. Dominios analíticos

### 2.1 Proceso
- tiempo entre asignación, inicio y logro;
- cumplimiento de secuencias;
- retrasos;
- reintentos;
- cuellos de botella;
- actividades vencidas;
- excepciones;
- carga de intervención humana.

### 2.2 Aprendizaje
- nodos con mayor dificultad;
- distribución de intentos;
- tipos de error;
- recuperación espaciada;
- progresión entre exposición, práctica, demostración y transferencia.

### 2.3 Ambientes
- capacidad utilizada;
- frecuencia de oportunidades clínicas;
- sustituciones;
- disponibilidad;
- diferencias de resultados según ambiente;
- carga sobre servicios y referentes.

### 2.4 Simulación
- nodos que requieren práctica adicional;
- número de repeticiones;
- errores frecuentes;
- desempeño antes y después de simulación;
- relación entre desempeño simulado y clínico.

### 2.5 Supervisión y EPA
- nivel de supervisión por EPA;
- tiempo hasta cambio de nivel;
- número y diversidad de observaciones;
- discrepancias entre observadores;
- necesidad de retorno a supervisión mayor.

### 2.6 Transferencia
- consistencia del desempeño durante los turnos;
- persistencia a 30/60 días;
- brechas entre aprobación inicial y práctica real;
- necesidades de refuerzo.

### 2.7 Operación
- tamaño de cohorte;
- horas de referentes;
- uso de ambientes;
- demanda de laboratorio;
- carga del equipo de Formación;
- capacidad máxima sostenible.

## 3. Niveles de indicador

1. **Evento:** qué ocurrió.
2. **Actividad:** cómo se ejecutó una actividad.
3. **Nodo:** avance y logro.
4. **Competencia:** cobertura e integración.
5. **EPA:** autonomía y supervisión.
6. **Trayectoria:** progreso longitudinal individual.
7. **Cohorte:** comportamiento agregado.
8. **Sistema:** capacidad, carga y efectividad.

## 4. Dimensiones mínimas

Los análisis deberían poder segmentarse, cuando sea apropiado, por:

- rol;
- servicio/unidad funcional;
- cohorte;
- competencia;
- nodo;
- experiencia;
- ambiente;
- versión;
- periodo;
- nivel de supervisión.

## 5. Principio de interpretación

No se utilizará una única métrica como proxy de competencia. Progreso, tiempo, nota o asistencia son señales parciales. La interpretación debe combinar evidencia de aprendizaje, desempeño y transferencia.

## 6. Gestión por excepción

Una de las salidas analíticas centrales será detectar:

- participantes fuera de ritmo;
- nodos con fallas repetidas;
- ambientes saturados;
- evidencias faltantes;
- discrepancias de supervisión;
- fallas recurrentes del diseño.

La analítica debe ayudar a decidir **dónde intervenir**, no solo producir reportes.

## 7. Evolución futura

Una vez exista suficiente volumen y calidad de datos podrán explorarse modelos de predicción o personalización. Estos no deben incorporarse antes de disponer de definiciones estables, trazabilidad y validación del proceso.
