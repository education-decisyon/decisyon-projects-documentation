---
icon: magnifying-glass
---

# 4. DeepFind

### Descripción general

**DeepFind** es un chatbot de IA integrado en DISS que permite a los usuarios consultar una Fuente de Conocimiento configurada — un repositorio de manuales de planta, procedimientos, FAQs, políticas, informes — usando lenguaje natural. DeepFind analiza los documentos que han sido cargados y sintetiza una respuesta basada en su contenido. Se pueden adjuntar múltiples documentos a la misma conversación para proporcionar un contexto más rico a la IA.

<figure><img src=".gitbook/assets/DeepFind-Cover Welcome page.png" alt=""><figcaption></figcaption></figure>

## Cuándo usarla

* Buscar el procedimiento para una intervención específica en un equipo.
* Verificar los requisitos previos o los pasos de una política de calidad o seguridad.
* Identificar un código de error que apareció en una máquina y encontrar las acciones correctivas recomendadas.
* Encontrar el párrafo correcto en un manual técnico extenso durante una investigación de Kata.

## Requisitos previos

* Debe configurarse una Fuente de Conocimiento para tu planta en DISS.
* Los documentos relevantes (manuales, procedimientos, FAQs, referencias de códigos de error) deben haberse cargado a la Fuente de Conocimiento.
* DeepFind debe estar explícitamente habilitado en esa Fuente de Conocimiento.

{% hint style="info" %}
Si DeepFind no es visible en tu barra de herramientas DISS, contacta a tu administrador DISS para verificar que se ha configurado una Fuente de Conocimiento con DeepFind habilitado para tu planta.
{% endhint %}

## Cómo usarla

{% stepper %}
{% step %}
### Configurar la Fuente de Conocimiento

* Este paso lo realiza un usuario con el ámbito de **administrador de Fuente de Conocimiento** y debe completarse antes de que los usuarios finales puedan consultar DeepFind.

<figure><img src=".gitbook/assets/diss_user-profile-details-with-knowledge-source-administrator-scope-highlighted.png" alt="Perfil de usuario con el ámbito de administrador de Fuente de Conocimiento destacado"><figcaption></figcaption></figure>

* Hacer clic en el avatar de usuario en la esquina superior derecha y seleccionar **Fuentes de Conocimiento** en el menú desplegable. En el panel izquierdo, hacer clic en **+** para abrir el diálogo de creación de fuente de conocimiento. Introducir un nombre descriptivo y hacer clic en **Crear**.

<figure><img src=".gitbook/assets/Knowledge Sources — profile dropdown showing the Knowledge Sources option.png" alt=""><figcaption></figcaption></figure>

* Con la Fuente de Conocimiento seleccionada, ir a la pestaña **Documentos** y hacer clic en **Importar archivo** para cargar los documentos relevantes (PDF o formato compatible). Repetir para cada archivo adicional.

<figure><img src=".gitbook/assets/knowledge-sources_documents-tab-with-import-file-button-and-uploaded-document-list.png" alt="Pestaña Documentos con el botón Importar archivo y la lista de documentos cargados"><figcaption></figcaption></figure>

* En la pestaña **Permisos**, asignar las organizaciones y grupos de usuarios autorizados a consultar esta Fuente de Conocimiento.

<figure><img src=".gitbook/assets/knowledge-sources_permissions-tab-with-organisation-and-group-configured.png" alt="Pestaña Permisos con organización y grupo configurados"><figcaption></figcaption></figure>

* En la pestaña **Agentes de IA**, habilitar el selector **DeepFind AI Assistant** para conectar esta Fuente de Conocimiento a DeepFind.

<figure><img src=".gitbook/assets/knowledge-sources_ai-agents-tab-with-deepfind-ai-assistant-enabled.png" alt="Pestaña Agentes de IA con DeepFind AI Assistant habilitado"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Abrir DeepFind

* Localizar el icono **DeepFind Assistant** en la barra de herramientas DISS y hacer clic para abrir la interfaz de chat.

<figure><img src=".gitbook/assets/deepfind_assistant-icon-in-the-toolbar.png" alt="Icono DeepFind Assistant en la barra de herramientas"><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/deepfind_chat-interface-opened-empty-state.png" alt="Interfaz de chat DeepFind abierta (estado vacío)"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Hacer una pregunta

* Escribir la pregunta en lenguaje natural — las frases completas funcionan mejor que las búsquedas por palabras clave. Para la resolución de problemas, incluir el código de error y una breve descripción del síntoma.

<figure><img src=".gitbook/assets/deepfind_typing-a-natural-language-question-with-error-code-example.png" alt="Escribiendo una pregunta en lenguaje natural con ejemplo de código de error"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Leer la respuesta y hacer seguimiento

* Leer la respuesta sintetizada. DeepFind cita el documento fuente y la sección al final de cada respuesta, para que puedas verificar de dónde proviene la información. Si es necesario, hacer una pregunta de seguimiento para refinar o ampliar la respuesta.

<figure><img src=".gitbook/assets/deepfind_synthesised-answer-and-follow-up-turn.png" alt="Respuesta sintetizada y turno de seguimiento"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lectura del resultado

DeepFind sintetiza una respuesta basada en los pasajes más relevantes encontrados en la Fuente de Conocimiento configurada y en los documentos adjuntos a la conversación. La respuesta respeta las políticas de acceso de los documentos subyacentes: un usuario solo ve información de los documentos a los que tiene acceso.

Cuando DeepFind no puede responder basándose en el material disponible, devuelve: _"Lo siento, pero no puedo ayudar con eso porque está fuera del alcance de mi conocimiento."_ Esto significa que no se encontró ningún documento relevante, no que el tema no exista.

## Consejos y límites conocidos

{% hint style="info" %}
* Hacer una pregunta a la vez — las preguntas compuestas tienden a responderse parcialmente.
* Si la respuesta es incompleta, reformular con diferentes palabras clave o ser más específico sobre el equipo, proceso o código de error.
* Si la pregunta está dentro del alcance pero no se encuentra respuesta, consultar al administrador DISS para verificar que el documento relevante está cargado y DeepFind está habilitado en esa Fuente de Conocimiento.
* DeepFind no inventa contenido: solo referencia material presente en la Fuente de Conocimiento configurada o en los documentos adjuntos.
{% endhint %}
