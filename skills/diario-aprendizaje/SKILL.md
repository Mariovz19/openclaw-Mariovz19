---
name: diario-aprendizaje
description: "Registra y organiza los aprendizajes diarios del usuario en su diario personal de Google Docs."
---

---
name: diario-aprendizaje
description: Registra y organiza los aprendizajes diarios del usuario en su diario personal de Google Docs.
---

# Diario de aprendizaje diario

## Objetivo

Transformar los aprendizajes del usuario en entradas organizadas y guardarlas en su documento personal de Google Docs.

## Cuándo utilizar esta skill

Activar cuando el usuario:
- Comparta lo que aprendió durante el día.
- Quiera registrar nuevos conocimientos.
- Solicite actualizar su diario de aprendizaje.
- Envíe una lista de conceptos, experiencias o ideas aprendidas.

## Input esperado

El usuario puede proporcionar información en lenguaje natural, texto libre o listas de puntos.

Ejemplo:

Hoy aprendí:
- Qué son los embeddings.
- Cómo funciona una base de datos vectorial.
- Cómo utilizar RAG para consultar documentos.
- La diferencia entre un LLM y un modelo de embeddings.

No es obligatorio que el usuario utilice un formato específico.

## Información de configuración

Consultar los archivos de configuración del workspace:

- USER.md: contexto académico y preferencias del usuario.
- SOUL.md: personalidad y estilo de comunicación.
- AGENTS.md: reglas y límites de comportamiento.
- TOOLS.md: servicios disponibles y destinos de almacenamiento.

Configuración regional:
- Zona horaria: America/Panama.
- Idioma: español.
- Fecha: utilizar la fecha local de Panamá.

## Flujo de ejecución

1. Recibir los aprendizajes proporcionados por el usuario.
2. Identificar los conceptos y conocimientos principales.
3. Organizar la información sin modificar su significado.
4. Generar una entrada estructurada.
5. Consultar TOOLS.md para localizar el Google Doc configurado.
6. Utilizar Zapier para acceder a Google Docs.
7. Añadir la nueva entrada al documento existente.
8. Verificar que la entrada se haya guardado correctamente.
9. Informar al usuario del resultado.

## Formato de salida

Cada entrada debe seguir esta estructura:

# Diario de aprendizaje - DD/MM/YYYY

## Aprendizajes del día

- Aprendizaje 1.
- Aprendizaje 2.
- Aprendizaje 3.

## Conceptos importantes

Explicación breve de los conceptos principales mencionados por el usuario.

## Reflexión del día

Breve reflexión basada exclusivamente en los aprendizajes proporcionados.

## Próximos pasos

Posibles acciones para profundizar en los conocimientos adquiridos, claramente identificadas como sugerencias.

## Destino

- Servicio: Google Docs.
- Documento: Diario de Aprendizaje.
- Identificador: consultar TOOLS.md.
- Acción: añadir una entrada al documento existente.

## Reglas importantes

- Nunca inventar aprendizajes.
- No eliminar entradas anteriores.
- No sobrescribir el documento completo.
- No registrar información que el usuario no haya proporcionado o confirmado.
- Evitar entradas duplicadas.
- Si el documento no existe o no se puede localizar, informar al usuario.
- No afirmar que se guardó una entrada sin verificarlo.

## Confirmación al usuario

Cuando la operación termine correctamente, responder:

"Tu aprendizaje de hoy ha sido registrado correctamente en tu Diario de Aprendizaje.

Fecha: DD/MM/YYYY

Aprendizajes registrados: [cantidad]

Documento: [enlace de Google Docs]"
