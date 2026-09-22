# 01. Modelo semántico: competencias y nodos

**Versión:** 0.1  
**Estado:** preliminar

## 1. Jerarquía canónica

TravesíaHOMI utiliza la siguiente jerarquía:

**Competencia crítica → Nodo → Experiencia → Actividad → Evidencia → Evaluación → Resultado → EPA → Nivel de supervisión → Transferencia**

Cada objeto tiene un significado diferente y no debe intercambiarse con otro.

## 2. Definiciones

### Competencia crítica
Capacidad amplia cuyo dominio inicial HOMI considera necesario para un ejercicio seguro del rol. Describe una capacidad de la persona, no una capacitación.

### Nodo
Unidad funcional mínima que compone una competencia. Debe ser suficientemente concreta para definir qué desempeño debe desarrollarse, qué experiencias lo favorecen y cómo se demuestra.

Un nodo **no es** un servicio, un curso, una charla, un recurso ni necesariamente una EPA.

### Experiencia
Tipo de situación de aprendizaje requerida por el nodo: estudio guiado, caso, observación, práctica deliberada, simulación, interacción con experto, discusión, ejecución supervisada, uso de sistema, evaluación o transferencia.

### Actividad
Instancia concreta que una persona debe realizar en un momento determinado.

### Evidencia
Huella observable producida por la actividad: comportamiento observado, caso resuelto, registro, lista de cotejo, producto, respuesta, archivo u otra evidencia válida.

### Evaluación
Proceso mediante el cual una evidencia se interpreta según un criterio.

### Resultado
Estado derivado de la evaluación: alcanzado, no alcanzado, requiere refuerzo, nivel de supervisión, etc.

### EPA
Actividad profesional auténtica que integra varios nodos y/o competencias y cuya responsabilidad puede confiarse progresivamente.

## 3. Competencias críticas candidatas v0.1

Actualmente se trabaja con diez dominios provisionales:

1. Integrarse y desempeñarse de forma segura dentro del sistema de enfermería HOMI.
2. Administrar medicamentos y terapias de manera segura.
3. Gestionar de manera segura accesos vasculares y terapia de infusión según el rol.
4. Gestionar de forma segura el ciclo transfusional.
5. Monitorizar al paciente pediátrico, reconocer deterioro y activar oportunamente la respuesta.
6. Prevenir infecciones y ejecutar cuidados con técnica segura.
7. Prevenir, identificar y responder al deterioro de la integridad cutánea.
8. Gestionar de forma segura muestras y apoyos diagnósticos.
9. Gestionar riesgos del cuidado, tecnologías y eventos de seguridad.
10. Proporcionar cuidado pediátrico humanizado y comunicarse con el niño y su familia en situaciones complejas.

Este listado es una hipótesis estructurada y debe contrastarse con lineamientos institucionales oficiales y validación de liderazgo.

## 4. Naturaleza pedagógica del nodo

Cada nodo debe clasificarse por una naturaleza predominante y, cuando sea necesario, una secundaria:

- **Conceptual-decisional:** comprender información y se usa para decidir.
- **Perceptivo-reconocedora:** identificar, discriminar y reconocer señales relevantes.
- **Procedimental-psicomotora:** ejecutar físicamente una secuencia con precisión y seguridad.
- **Operativo-sistémica:** desenvolverse correctamente dentro de procesos y sistemas institucionales.
- **Comunicacional-relacional:** interactuar de manera efectiva con pacientes, familias o equipo.
- **Colaborativo-coordinativa:** coordinar acciones con otras personas y roles.
- **Integrador-clínica:** combinar capacidades previas en una situación completa.
- **Transferencia al puesto:** demostrar desempeño consistente en trabajo real.

La naturaleza describe **qué tipo de aprendizaje exige el nodo**, no dónde se enseñará.

## 5. Función arquitectónica del nodo

Un nodo puede cumplir una de estas funciones principales:

- **Basal:** prerrequisito reutilizable por múltiples nodos o competencias.
- **Específico:** propio de una competencia.
- **Aplicativo:** utiliza aprendizajes previos para ejecutar una acción en contexto.
- **Integrador:** combina varios nodos en una situación compleja.
- **Transferencial:** verifica desempeño sostenido en el puesto.

## 6. Caracterización mínima de un nodo

Todo nodo debe disponer, progresivamente, de:

- ID canónico;
- nombre;
- competencia;
- versión y estado;
- propósito de desempeño;
- naturaleza principal/secundaria;
- función;
- alcance por rol;
- nivel esperado por rol;
- prerrequisitos;
- riesgo;
- frecuencia clínica;
- predictibilidad;
- necesidad de repetición;
- necesidad de estandarización;
- consecuencia del error;
- experiencias requeridas;
- ambientes posibles;
- función en simulación;
- evidencia;
- criterio de logro;
- recuperación de la información/espaciamiento;
- continuidad durante los turnos;
- posibles EPA relacionadas.

## 7. Piel como primera validación clínica parcial

La competencia de integridad cutánea ha sido revisada con liderazgo experto y actualmente incluye:

- C07-N01 Valoración del riesgo y de la piel.
- C07-N02 Cuidados generales de lesiones y heridas.
- C07-N03 Prevención de lesiones asociadas a dispositivos, adhesivos, presión y humedad.
- C07-N04 Manejo y cuidado integral de férulas y yesos.
- C07-N05 Cuidado integral de ostomías y dispositivos asociados.
- C07-N06 Escalamiento y consulta.
- C07-N07 Registro y seguimiento.

La validación clínica confirma el nodo; la arquitectura pedagógica todavía puede ajustar naturaleza, función, experiencias y evidencias.

## 8. Regla de calidad

Antes de aceptar un nodo debe poder responderse:

- ¿describe un desempeño observable?
- ¿es crítico para el periodo de incorporación?
- ¿tiene límites claros?
- ¿es independiente o debería ser parte de otro nodo?
- ¿puede asociarse a experiencias y evidencia?
- ¿su granularidad es comparable con la de nodos equivalentes?
