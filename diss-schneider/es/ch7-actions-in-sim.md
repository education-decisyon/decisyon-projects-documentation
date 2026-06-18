---
icon: list-check
---

# 7. Actions in SIM

### Descripción general

La función **Acciones** en DISS es la forma estructurada de registrar, asignar y hacer seguimiento de actividades correctivas y de mejora directamente desde los SIM Boards. Aquí se documentan dos casos de uso complementarios: **Crear acción** — para registrar una nueva acción con todo el contexto SIM — y **Editar acción** — para mantener una acción existente actualizada mientras el equipo la resuelve durante la rutina diaria SIM.

<figure><img src=".gitbook/assets/Action - Overview (1).png" alt=""><figcaption></figcaption></figure>

## Cuándo usarla

* Abrir una **Crear acción** durante una reunión SIM cuando se identifica un problema u oportunidad en la línea: un problema de Seguridad / Calidad / Entrega / Mantenimiento / Producción / Ingeniería con un responsable claro y una fecha límite.
* Abrir una **Editar acción** entre reuniones SIM para mantener una acción actualizada: progresión del estado, descripción refinada, nuevos adjuntos, soluciones capturadas o notas añadidas al Registro de actividad.
* Usar Acciones en SIM para garantizar que cada problema identificado en un SIM Board se convierte en una actividad trazable y asignable, en lugar de quedar como un compromiso verbal.

## Requisitos previos

* El usuario debe tener acceso a los SIM Boards en los que están habilitadas las Acciones.
* Las categorías de acción, áreas de producción y líneas deben estar configuradas en **Configuración de planta** — rellenan los campos Categoría, Módulo y Línea en el formulario Crear acción.
* El Responsable o Equipo debe existir en DISS para poder asignarse a la acción.

## Cómo usarla — Crear acción

{% stepper %}
{% step %}
### Abrir el formulario Crear acción

* Desde el SIM Board, abrir el formulario **Crear acción**.

<figure><img src=".gitbook/assets/create-action_entry-point-on-the-sim-board.png" alt="Punto de entrada Crear acción en el SIM Board"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Configurar el contexto SIM

Configurar el contexto SIM:

* **Categoría** (Seguridad, Calidad, Entrega, Mantenimiento, Producción, Ingeniería);
* **Módulo** (precargado con el Área de producción del tablero de origen);
* **Línea**.
* El **nivel SIM de origen** y el **nivel SIM objetivo** se seleccionan automáticamente del SIM Board de origen; verificarlos antes de guardar ya que el nivel SIM de origen se vuelve inmutable una vez guardado.

<figure><img src=".gitbook/assets/create-action_sim-context-bar-category.png" alt="Barra de contexto SIM de Crear acción con Categoría"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Escribir el Título

* Escribir un **Título** que identifique el problema (máx. 500 caracteres).

<figure><img src=".gitbook/assets/create-action_title-field.png" alt="Campo Título de Crear acción"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Configurar el Estado

* Dejar el **Estado** como "Nuevo" a menos que el proceso SIM local requiera un estado inicial diferente.

<figure><img src=".gitbook/assets/create-action_status-dropdown.png" alt="Desplegable Estado de Crear acción"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Escribir la Descripción

* Escribir la **Descripción**. Usar negrita, cursiva y listas para mayor legibilidad.
* Opcionalmente hacer clic en **AI Enhance** para mejorar la claridad; el indicador de calidad proporciona retroalimentación en tiempo real mientras se escribe.

<figure><img src=".gitbook/assets/create-action_description-with-ai-enhance-and-quality-indicator.png" alt="Descripción con AI Enhance e indicador de calidad"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Establecer la Fecha límite

* Seleccionar una **Fecha límite** — por defecto hoy + 7 días.

<figure><img src=".gitbook/assets/create-action_due-date-picker.png" alt="Selector de Fecha límite de Crear acción"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Establecer Prioridad y Gravedad

* Establecer la **Prioridad** (Trivial / Menor / Mayor / Crítica / Bloqueante)
* Establecer la **Gravedad** (Baja / Media / Alta / Crítica)

<figure><img src=".gitbook/assets/create-action_priority-and-severity-dropdowns.png" alt="Desplegables de Prioridad y Gravedad"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Asignar Iniciador, Equipo y Responsable

* Confirmar el **Iniciador** (precargado con el usuario actual; cambiar solo cuando se registra en nombre de otro).
* Asignar responsabilidad: al menos uno entre **Equipo** y **Responsable** debe estar configurado para que la acción tenga una parte claramente responsable en el SIM Board.

<figure><img src=".gitbook/assets/create-action_team-and-owner-assignment.png" alt="Asignación de Equipo y Responsable"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Guardar la acción

* Hacer clic en **Guardar acción**.
* El botón verde se activa solo cuando todos los campos obligatorios están completados. Una vez guardada, la acción es visible en el SIM Board.

<figure><img src=".gitbook/assets/create-action_save-action-button-active-and-action-visible-on-sim-board.png" alt="Botón Guardar acción activo y acción visible en el SIM Board"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Cómo usarla — Editar acción

Editar acción tiene **guardado automático**: cada campo se confirma individualmente al salir del campo. No hay botón de guardado global — el encabezado muestra "Todos los cambios guardados" como confirmación. Este comportamiento permite realizar actualizaciones rápidamente durante la reunión SIM sin interrumpir el ritmo de la misma.

{% stepper %}
{% step %}
### Abrir la acción desde el SIM Board

* Desde el SIM Board, abrir la acción que se desea actualizar.

<figure><img src=".gitbook/assets/edit-action_opening-an-action-from-the-sim-board.png" alt="Abriendo una acción desde el SIM Board"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Actualizar los campos del Panel de entrada

* Actualizar los campos editables en el Panel de entrada: **Título, Estado, Descripción** (con AI Enhance e indicador de calidad), **Fecha límite, Prioridad, Gravedad, Iniciador, Equipo, Responsable, Adjuntos**.

<figure><img src=".gitbook/assets/edit-action_entry-panel-with-all-editable-fields.png" alt="Panel de entrada con todos los campos editables"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Escalar a un nivel SIM superior si es necesario

* Cambiar el **Nivel SIM objetivo** en la barra de contexto si la acción necesita escalar (es el único campo de la barra de contexto que permanece editable tras la creación).

<figure><img src=".gitbook/assets/edit-action_target-tier-dropdown-in-the-context-bar.png" alt="Desplegable Nivel SIM objetivo en la barra de contexto"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Añadir o revisar Soluciones y Propuestas

* En el panel **Soluciones y propuestas**, escribir o pegar la solución propuesta, o hacer clic en **AI Suggest** para generar automáticamente propuestas de solución puntuadas por relevancia.

<figure><img src=".gitbook/assets/edit-action_solutions-proposals-with-ai-suggest.png" alt="Soluciones y propuestas con AI Suggest"><figcaption></figcaption></figure>

* Las propuestas se extraen de los documentos cargados en la **Fuente de Conocimiento Deep Find**.

<figure><img src=".gitbook/assets/edit-action_solutions-proposals-from-deepfind-document.png" alt="Soluciones y propuestas extraídas de la Fuente de Conocimiento DeepFind"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Añadir notas al Registro de actividad

* Añadir notas al **Registro de actividad** en la parte inferior del panel; adjuntar archivos mediante el icono de clip si es necesario. El Registro de actividad es el historial completo de la acción en el SIM Board.

<figure><img src=".gitbook/assets/edit-action_activity-log-with-note-input-and-paperclip.png" alt="Registro de actividad con entrada de nota y clip"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Establecer la acción como Completada

* Establecer el **Estado** a "Completado" solo cuando la acción esté genuinamente finalizada: "Completado" bloquea el registro completo.

<figure><img src=".gitbook/assets/edit-action_status-set-to-done-locked-record.png" alt="Estado establecido como Completado — registro bloqueado"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lectura del resultado

* **Indicador de calidad** en la Descripción — Deficiente / Aceptable / Bueno / Excelente — señala si el texto contiene suficiente información para ser accionable
* **AI Enhance** reescribe el texto para mayor claridad profesional; siempre revisar el resultado antes de guardar.
* **AI Suggest** en Soluciones clasifica las propuestas por porcentaje de relevancia respecto al contenido de la Descripción.
* Se envían notificaciones por correo electrónico al cambiar el estado, nueva asignación de Equipo/Responsable, aviso de fecha límite a 48 horas y acciones vencidas.

## Consejos y límites conocidos

{% hint style="info" %}
* No establecer el Estado como "Completado" hasta que la acción esté genuinamente finalizada: no se puede editar después.
* Si tanto el Equipo como el Responsable se eliminan, el guardado falla — mantener siempre al menos uno asignado.
* El guardado automático revierte el campo en caso de error: verificar la conexión de red si aparece un mensaje de error de guardado.
* AI Enhance y AI Suggest son asistivos: el Responsable sigue siendo el responsable del redactado final y la solución elegida.
* La escalada entre niveles SIM se realiza cambiando el Nivel SIM objetivo, no creando una nueva acción — esto preserva el historial del Registro de actividad del problema original.
{% endhint %}
