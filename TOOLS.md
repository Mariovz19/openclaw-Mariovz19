# TOOLS.md

## Entorno disponible

El agente OpenClaw está instalado en un VPS.

Dispone de una conexión activa con Zapier que permite interactuar con diferentes servicios.

Telegram funciona como canal principal de comunicación entre el usuario y el agente.

## Zona horaria y fechas

- Utilizar siempre la zona horaria `America/Panama`.
- Registrar las entradas del diario con la fecha local de Panamá.
- Crear y consultar eventos de Google Calendar utilizando la hora local de Panamá.
- No utilizar UTC como hora visible para el usuario.
- Evitar confusiones entre fechas UTC y fechas locales.

## Herramientas conectadas

### 1. Google Docs

**Uso principal:** Crear y organizar documentos.

**Utilizar para:**
- Registrar el diario de aprendizaje.
- Crear documentos con notas de reuniones.
- Organizar información de estudio.
- Documentar proyectos.

**Convenciones:**
- Utilizar títulos descriptivos.
- Incluir fechas cuando corresponda.
- Mantener una estructura organizada.
- No sobrescribir documentos existentes sin autorización.

### 2. Google Drive

**Uso principal:** Almacenar y organizar documentos.

**Utilizar para:**
- Guardar notas de reuniones.
- Organizar documentos relacionados con el bootcamp.
- Mantener los archivos de aprendizaje.

**Convenciones:**
- Evitar archivos duplicados.
- Utilizar nombres claros.
- Respetar las carpetas existentes.
- No inventar rutas o carpetas que no estén configuradas.

### 3. Google Calendar

**Uso principal:** Gestionar compromisos y eventos.

**Utilizar para:**
- Consultar eventos.
- Organizar sesiones de estudio.
- Gestionar compromisos académicos.

**Convenciones:**
- Comprobar fecha y hora antes de crear eventos.
- Utilizar la zona horaria configurada en la cuenta.
- Solicitar confirmación antes de modificar o cancelar eventos existentes.

### 4. Gmail

**Uso principal:** Gestionar información recibida por correo electrónico.

**Utilizar para:**
- Consultar correos cuando el usuario lo solicite.
- Identificar información académica relevante.
- Extraer información para tareas de organización.

**Convenciones:**
- No enviar correos sin autorización.
- No eliminar correos.
- Mantener la privacidad de los mensajes.

### 5. Google Tasks

**Uso principal:** Gestionar tareas pendientes.

**Utilizar para:**
- Consultar tareas.
- Organizar actividades.
- Identificar pendientes relacionados con el estudio y proyectos.

**Convenciones:**
- Utilizar descripciones claras.
- No duplicar tareas.
- No marcar tareas como completadas sin confirmación o evidencia.

### 6. GitHub

**Uso principal:** Gestionar proyectos y repositorios de código.

**Utilizar para:**
- Consultar repositorios.
- Revisar issues y commits.
- Documentar proyectos.
- Apoyar el desarrollo de proyectos del bootcamp.

**Convenciones:**
- No modificar código ni repositorios sin autorización.
- No publicar cambios sin permiso.
- Mantener una documentación clara.

### 7. Telegram

**Uso principal:** Canal principal de comunicación con el usuario.

**Utilizar para:**
- Recibir instrucciones.
- Enviar confirmaciones.
- Compartir resúmenes.
- Comunicar resultados de automatizaciones.

**Convenciones:**
- Mantener mensajes breves y claros.
- Proporcionar enlaces a documentos cuando estén disponibles.
- Informar cuando una operación falle.

## Skills personalizadas

### Skill 1: Diario de aprendizaje diario

**Herramientas:** Telegram y Google Docs.

**Flujo de trabajo:**

1. Recibir los aprendizajes del usuario por Telegram.
2. Interpretar y organizar la información.
3. Generar una entrada con fecha y título.
4. Añadir los aprendizajes y una breve reflexión.
5. Guardar la entrada en el Google Doc correspondiente.
6. Confirmar la operación y compartir el enlace.

**Destino:** Documento de Google Docs destinado al diario personal de aprendizaje.

### Skill 2: Notas de reunión

**Herramientas:** Telegram y Google Drive / Google Docs.

**Flujo de trabajo:**

1. Recibir los apuntes de la reunión.
2. Analizar y organizar el contenido.
3. Identificar el resumen, las decisiones, las tareas y las preguntas abiertas.
4. Crear un documento estructurado.
5. Guardarlo en Google Drive.
6. Confirmar la operación y compartir el enlace.

**Destino:** Google Drive, mediante un nuevo documento de Google Docs.

## Reglas generales de utilización

- Utilizar la herramienta más adecuada para cada tarea.
- No asumir que una integración está disponible si no se ha comprobado.
- No inventar resultados de operaciones.
- Comprobar que los documentos se hayan creado o actualizado correctamente.
- Evitar duplicar información.
- Informar al usuario cuando una operación necesite autorización.
- Priorizar la automatización de tareas repetitivas relacionadas con el aprendizaje y la productividad.
