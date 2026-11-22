Diseño de Skills para OpenClaw

Este documento describe el diseño de dos skills que se implementarán en OpenClaw. Cada skill tiene un propósito específico, requiere información sencilla del usuario y genera resultados que se pueden guardar y consultar posteriormente.
________________________________________________________________________________________

1. Diario de aprendizaje diario
¿Qué hace esta skill?

Recibe los aprendizajes del día, los organiza y añade una entrada estructurada a un Google Doc que funciona como diario personal de conocimiento.

¿Qué input necesita el agente?
Una lista de los aprendizajes del día en texto o viñetas.
Puede incluir conceptos nuevos, ideas, experiencias o conocimientos adquiridos.
A partir de los cinco archivos de configuración, el agente ya conoce la identidad y preferencias del usuario, sus instrucciones de comportamiento, las herramientas disponibles y la configuración necesaria para trabajar.
No es necesario indicar nuevamente dónde guardar la información si el destino ya está configurado.

¿Cómo es un buen output?
Formato: Entrada organizada con fecha, título, aprendizajes principales y una breve reflexión.
Destino: Un Google Doc utilizado como diario personal de aprendizaje.

Cómo sabré que funcionó: La nueva entrada aparece correctamente en el documento, con la fecha correspondiente y sin eliminar las entradas anteriores.

2. Notas de reunión
¿Qué hace esta skill?

Transforma apuntes desordenados de una reunión en un resumen organizado con decisiones, tareas pendientes y preguntas abiertas.

¿Qué input necesita el agente?
Apuntes de la reunión escritos en texto, aunque estén desordenados.
Puede incluir nombres de participantes, temas tratados, acuerdos y tareas.
A partir de los cinco archivos de configuración, el agente ya conoce las instrucciones de comportamiento, las herramientas disponibles y las preferencias para organizar y guardar información.
No es necesario proporcionar instrucciones detalladas sobre cómo estructurar las notas en cada ejecución.

¿Cómo es un buen output?
Formato: Documento dividido en cuatro secciones:
Resumen de la reunión.
Decisiones tomadas.
Tareas pendientes y responsables.
Preguntas abiertas.
Destino: Google Drive, guardado como un nuevo documento de Google Docs.

Cómo sabré que funcionó: El documento aparece en Drive con un título identificable, las secciones completas y las tareas claramente asignadas cuando se conoce al responsable.
Criterios generales de diseño
Las dos skills deben poder ejecutarse varias veces.
El agente debe interpretar texto natural sin exigir formatos complicados.
Los documentos nuevos deben conservar la información anterior.
Los resultados deben ser claros, ordenados y fáciles de consultar.
El agente debe confirmar cuando una operación se complete correctamente.
