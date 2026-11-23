---
name: notas-reunion
description: "Convierte apuntes de reuniones en documentos estructurados."
---

# Notas de reunión

## Objetivo

Convertir apuntes desordenados de reuniones en documentos claros y estructurados, guardados en Google Drive mediante Google Docs.

## Cuándo utilizar esta skill

Activar cuando el usuario:
- Comparta apuntes de una reunión.
- Solicite organizar notas de una reunión.
- Quiera identificar decisiones y compromisos.
- Necesite extraer tareas pendientes de una conversación.
- Solicite generar un resumen de una reunión.

## Input esperado

El usuario puede proporcionar:
- Apuntes escritos en texto libre.
- Listas de ideas.
- Decisiones tomadas.
- Nombres de participantes.
- Tareas y compromisos.
- Preguntas pendientes.

No es obligatorio utilizar un formato específico.

Ejemplo:

Reunión del proyecto de IA:

- Revisamos el avance del proyecto.
- Carlos trabajará en la integración de la API.
- María revisará los resultados del modelo.
- Se acordó entregar el prototipo el viernes.
- Falta decidir qué base de datos utilizaremos.

## Información de configuración

Consultar los archivos de configuración del workspace:

- USER.md: contexto académico y proyectos actuales.
- SOUL.md: personalidad y estilo de comunicación.
- AGENTS.md: reglas y límites de comportamiento.
- TOOLS.md: servicios disponibles y destinos de almacenamiento.

Configuración regional:
- Zona horaria: America/Panama.
- Idioma: español.
- Fecha: utilizar la fecha local de Panamá.

## Flujo de ejecución

1. Recibir los apuntes de la reunión.
2. Analizar y clasificar la información.
3. Identificar los temas principales.
4. Extraer las decisiones tomadas.
5. Identificar tareas pendientes y responsables cuando estén especificados.
6. Identificar preguntas abiertas.
7. Generar un documento estructurado.
8. Consultar TOOLS.md para localizar la carpeta de destino.
9. Utilizar Zapier para crear un nuevo Google Doc.
10. Guardar el documento en la carpeta correspondiente de Google Drive.
11. Verificar que el documento se haya creado correctamente.
12. Compartir el enlace con el usuario.

## Formato de salida

# Notas de reunión - AAAA-MM-DD - Tema

## 1. Información general

- Fecha:
- Tema:
- Participantes:
- Objetivo de la reunión:

Si algún dato no está disponible, indicarlo como "No especificado".

## 2. Resumen de la reunión

Descripción breve de los temas tratados y los puntos más importantes.

## 3. Decisiones tomadas

- Decisión 1.
- Decisión 2.

Incluir únicamente decisiones confirmadas durante la reunión.

## 4. Tareas pendientes

| Tarea | Responsable | Fecha límite | Estado |
|---|---|---|---|
| Descripción | Nombre | Fecha o no especificada | Pendiente |

No inventar responsables ni fechas.

## 5. Preguntas abiertas

- Pregunta 1.
- Pregunta 2.

Incluir los temas que todavía necesitan aclaración o una decisión.

## 6. Próximos pasos

Lista de acciones recomendadas para dar continuidad a los acuerdos.

Diferenciar las recomendaciones de los compromisos confirmados.

## Destino

- Servicio: Google Drive y Google Docs.
- Carpeta: Notas de Reuniones.
- Identificador: consultar TOOLS.md.
- Acción: crear un documento nuevo por cada reunión.

Formato del nombre:

Notas de reunión - AAAA-MM-DD - Tema

## Reglas importantes

- No inventar información.
- No convertir sugerencias en decisiones confirmadas.
- No asignar tareas a personas sin evidencia.
- No inventar fechas límite.
- Mantener el significado original de los apuntes.
- No eliminar documentos existentes.
- Crear un documento independiente por reunión.
- Si faltan datos, utilizar "No especificado".
- Si no se puede guardar el documento, informar al usuario.
- No afirmar que se creó el documento sin verificarlo.

## Confirmación al usuario

Cuando la operación termine correctamente, responder:

"Las notas de la reunión se han organizado y guardado correctamente.

Documento: [nombre del documento]

Ubicación: Google Drive / Notas de Reuniones

Enlace: [enlace de Google Docs]

Tareas identificadas: [cantidad]

Decisiones registradas: [cantidad]"
