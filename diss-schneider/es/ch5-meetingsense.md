---
icon: microphone
---

# 5. Análisis de Reunión

### Descripción general

**Análisis de Reunión** es la capacidad de grabación y transcripción de reuniones integrada en DISS. Transforma el diálogo hablado de una reunión SIM en datos digitales estructurados: una transcripción textual, un resumen ejecutivo, los problemas planteados y una lista de acciones propuestas listas para añadirse al plan de acción SIM. La sesión se contextualiza automáticamente con los metadatos del SIM Board desde el que se lanzó (Planta, nivel SIM, Área de producción) para que cada resultado esté ya vinculado al ámbito operativo correcto.

<figure><img src=".gitbook/assets/recording-widget-in-active-state-during-the-meeting-with-session-duration-and-audio-status-indicator.png" alt=""><figcaption></figcaption></figure>

## Cuándo usarla

* Durante una reunión diaria SIM 2 donde el equipo discute problemas, causas raíz y acciones correctivas y quiere que cada resultado sea trazable en DISS sin toma de notas manual.
* Cuando el Líder SIM quiere que la conversación quede grabada íntegramente para que nada se pierda entre la discusión y el plan de acción.
* Cuando el equipo necesita tanto un registro de asistencia como un conjunto estructurado de acciones listas para asignar de una vez al final de la reunión.

## Requisitos previos

* El SIM Board en el que se abre la reunión debe ser un **SIM 2** Board (Análisis de Reunión está habilitado en este nivel SIM).
* Debe haber un micrófono funcionando en el dispositivo utilizado para iniciar la reunión.
* Los roles de asistencia deben estar configurados para el SIM 2 Board — accesible en **Configuración de planta → Asistencia → Configuración de asistencia SIM 2.**
* El usuario debe tener permiso para iniciar una reunión en el SIM Board en cuestión.

## Cómo usarla

{% stepper %}
{% step %}
### Abrir el SIM Board e iniciar la reunión

* Navegar al SIM Board donde tiene lugar la reunión (**Digitized Idea & SIM System → SIM Boards → SIM 2**). La Planta, el Área de producción y la Fecha se rellenan automáticamente.
* Hacer clic en **Iniciar reunión** en la esquina superior derecha para abrir el diálogo de inicialización de la reunión.

<figure><img src=".gitbook/assets/sim-board-with-start-meeting-button-highlighted-in-the-top-right-corner.png" alt="SIM Board con el botón Iniciar reunión destacado"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Inicializar asistencia y Líder SIM

En el diálogo de inicialización:

* Definir el estado de cada participante (**A tiempo, Tarde, Ausente** o **No requerido**);
* Asignar el **Líder SIM** (por defecto el usuario actual, modificable mediante desplegable);
* Hacer clic en **Iniciar reunión** para continuar.

<figure><img src=".gitbook/assets/meeting-initialisation-dialog-attendance-statuses-and-sim-leader-selector.png" alt="Diálogo de inicialización de reunión con estados de asistencia y selector de Líder SIM"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Seleccionar la entrada de audio e iniciar la grabación

* Elegir el micrófono deseado de la lista de entradas de audio disponibles y confirmar. Si no se detecta ningún micrófono, se muestra un mensaje de error y la grabación no puede iniciarse.

<figure><img src=".gitbook/assets/audio-input-device-selection-popup-with-a-microphone-confirmed.png" alt="Popup de selección de dispositivo de entrada de audio con micrófono confirmado"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Realizar la reunión

Hablar con claridad durante toda la reunión y articular los elementos necesarios para crear acciones después:

* Una **breve descripción** del problema;
* La **Categoría** relevante (Seguridad, Calidad, Entrega, Mantenimiento, Producción, Ingeniería);
* El **nombre de la persona asignada**;
* La fecha **objetivo** de finalización.

<figure><img src=".gitbook/assets/recording-widget-in-active-state-during-the-meeting-with-session-duration-and-audio-status-indicator.png" alt="Widget de grabación en estado activo, con duración de sesión e indicador de estado de audio"><figcaption></figcaption></figure>

{% hint style="info" %}
Un tiempo de espera predefinido protege contra reuniones dejadas abiertas por error: un diálogo de notificación aparece dos minutos antes del tiempo de espera para dar la oportunidad de ampliar o detener la sesión manualmente.
{% endhint %}
{% endstep %}

{% step %}
### Detener la grabación

* Hacer clic en el control **Detener** cuando la reunión haya concluido. El sistema comienza a procesar el audio en segundo plano. Mientras se genera la transcripción, se puede cambiar a otras actividades — el equipo no necesita esperar en la página de la reunión.
* Una notificación confirma cuando el transcript y el análisis de IA están listos.

<figure><img src=".gitbook/assets/recording-stopped-processing-indicator-and-confirmation-that-transcription-is-queued.png" alt="Grabación detenida, indicador de procesamiento y confirmación de que la transcripción está en cola"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Abrir la reunión desde el archivo

* Navegar a **Reunión → Overview Meeting**.
* La página Overview Meeting lista cada sesión grabada en orden cronológico, mostrando título, nivel SIM, fecha y Líder SIM.

<figure><img src=".gitbook/assets/overview-meeting-archive-with-the-list-of-recorded-sessions.png" alt="Archivo Overview Meeting con la lista de sesiones grabadas"><figcaption></figcaption></figure>

* Hacer clic en una reunión para abrir su vista detallada.

<figure><img src=".gitbook/assets/meeting-detail-view_summary-identified-issues-ai-suggested-actions.png" alt="Vista detallada de reunión: Resumen, Problemas identificados, Acciones sugeridas por IA, duración, registro de asistencia"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Revisar y editar el transcript

* Hacer clic en **Mostrar transcripción** para mostrar el texto literal, que permanece completamente editable.
* Corregir cualquier malinterpretación del motor de voz a texto o añadir detalles que no se capturaron.
* Cuando el transcript se actualice, hacer clic en **Generar notas de reunión** para actualizar el resumen de IA.

<figure><img src=".gitbook/assets/transcript-pane-with-show-transcription-opened-and-generate-meeting-notes-button.png" alt="Panel de transcripción con Mostrar transcripción abierto y el botón Generar notas de reunión"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lectura del resultado

| Bloque                   | Descripción                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| Resumen                  | Una visión general narrativa de la discusión de la reunión generada por la IA, que cubre los principales temas abordados.       |
| Problemas identificados  | Una lista estructurada de problemas y anomalías identificados durante la reunión, extraídos por la IA de la conversación grabada. |
| Acciones sugeridas por IA | Propuestas de acción generadas automáticamente a partir del diálogo, cada una con una descripción inferida, categoría, responsable y fecha límite. |
| Registro de asistencia   | La lista de asistencia compilada al inicio de la reunión, con el estado establecido para cada participante.                     |
| Duración                 | La duración total de la sesión de reunión grabada.                                                                              |

## Consejos y límites conocidos

{% hint style="info" %}
* Hablar con claridad y evitar voces superpuestas: la calidad de extracción de IA escala con la claridad del audio.
* Mencionar nombres y fechas con precisión — "Juan, para el viernes" produce una sugerencia de IA más sólida que referencias implícitas como "él, para fin de semana".
* La Categoría y el Responsable son obligatorios para la creación de acciones: una acción propuesta sin esos valores debe completarse en la tabla de validación antes de poder guardarse.
* Análisis de Reunión es un asistente de grabación: el Líder SIM siempre tiene el control — las acciones forman parte del plan SIM solo después de una validación explícita, y el transcript puede editarse y resumirse de nuevo antes de crear cualquier acción.
{% endhint %}
