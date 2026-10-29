# Política de privacidad de Wabri — Web Agent Bridge

Vigente desde el 28 de octubre de 2026.

Wabri es una extensión de Chrome que conecta el chat de IA que tú elijas (Copilot Chat, ChatGPT o DeepSeek) con una página que tú vinculas, para automatizar tareas **paso a paso y bajo tu supervisión**. Wabri no tiene servidores propios: **el desarrollador no recibe, no guarda y no vende ningún dato**.

## Qué datos usa Wabri y para qué

| Dato | Para qué | A dónde va |
|---|---|---|
| Contenido de la página que vinculas: textos de botones, campos, enlaces y avisos visibles | Que el chat de IA sepa qué hay en la pantalla y decida el siguiente paso | Al chat de IA que elegiste, **dentro de tu propia sesión** en ese sitio, como si tú lo escribieras |
| Tu objetivo y tus indicaciones | Describir la tarea al chat de IA | Al mismo chat de IA |
| Estructura de los archivos que adjuntas (nombres de tablas, hojas y columnas) | Que el agente use los nombres correctos | Al chat de IA. **Los valores de las celdas nunca se leen ni se envían** |

Wabri **nunca** envía al chat de IA el valor de contraseñas, campos ocultos, números de tarjeta ni códigos de un solo uso.

Lo que el chat de IA haga con lo que recibe se rige por la política de privacidad de ese servicio (Microsoft, OpenAI o DeepSeek), igual que si tú escribieras en él.

## Qué se guarda en tu navegador

Todo queda **solo en tu navegador** (`chrome.storage`). Nada se sincroniza con tu cuenta de Google ni se envía a otro lugar:

- **Conversación y estado de la tarea**: se borran al cerrar Chrome o con «Nueva conversación».
- **Punto de control de la tarea** (objetivo, avance resumido y sitio, sin contenido de la página ni valores de campos): permite retomar una tarea interrumpida. Caduca a las 24 horas y se borra al terminar la tarea.
- **Aprendizajes que tú apruebas**: notas cortas sobre cómo se usa la interfaz de un sitio. Solo se guardan si pulsas «Guardar» y puedes borrarlos cuando quieras. Una validación rechaza notas con enlaces, correos, números largos, código o instrucciones sospechosas.
- **Métricas de tus últimas tareas** (sitio, objetivo resumido, pasos y errores): para que veas si el agente mejora. Se borran solas a los 7 días y puedes borrarlas antes desde el panel.
- **Configuración**: skills propias, skills activas y webhooks permitidos.

En la sección **«Tus datos»** del panel, el botón **«Borrar todos mis datos»** elimina todo lo anterior de una vez. Al desinstalar la extensión, Chrome también lo borra todo.

## Compartir

Wabri solo comparte datos cuando tú lo decides:

- **Exportar aprendizajes** genera un archivo en tu computador. Tú eliges si se lo envías a alguien.
- **Webhooks**: si agregas un origen en «Webhooks permitidos», el agente puede enviarle datos de la tarea a ese origen (solo `https`). Por defecto no hay ninguno y la función está apagada.

## Permisos de Chrome

- **Panel lateral, pestañas y grupos de pestañas**: mostrar el panel, saber qué pestaña vas a vincular y agrupar las pestañas de la tarea.
- **Acceso a sitios**: los tres chats de IA y, solo cuando pulsas «Vincular», el sitio que vinculas (Chrome te lo pregunta).
- **Scripting**: leer y operar la página vinculada.
- **Depurador (`debugger`)**: hacer clics y escribir como una persona en la pestaña vinculada, mientras una tarea corre. Chrome lo muestra con la barra «está depurando este navegador». No se usa para leer cookies, tráfico de red ni para ejecutar código.
- **Almacenamiento**: guardar lo descrito arriba en tu navegador.

## Sin telemetría ni código remoto

Wabri no incluye analítica, rastreo ni registros remotos, y no descarga ni ejecuta código de internet.

## Marcas

Wabri es un proyecto independiente y **no está afiliado** a Microsoft, OpenAI ni DeepSeek. Sus nombres se usan solo para indicar con qué servicios funciona.

## Cambios y contacto

Si esta política cambia, se actualizará este documento junto con la versión de la extensión. Para preguntas, abre un issue en https://github.com/Zitr0/wabri/issues.
