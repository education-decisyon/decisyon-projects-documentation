---
icon: chart-line
---

# 6. Perspectivas de Reunión

### Descripción general

Perspectivas de Reunión es un agente de IA que trabaja sobre las reuniones ya capturadas por Análisis de Reunión. Mientras Análisis de Reunión se centra en una única grabación, Perspectivas de Reunión analiza múltiples transcripciones de reuniones simultáneamente para identificar patrones, problemas recurrentes y acciones agregadas en todo el archivo. Transforma un flujo de actas SIM individuales en inteligencia operativa a nivel de planta o área.

<figure><img src=".gitbook/assets/meeting-insight_action-items-list-aggregated-across-meetings.png" alt=""><figcaption></figcaption></figure>

## Cuándo usarla

* Para responder "¿Qué problemas siguen recurriendo?" — Perspectivas de Reunión identifica temas recurrentes en las reuniones SIM durante un período elegido.
* Para producir una lista consolidada de acciones de muchas reuniones (por ejemplo, todas las reuniones SIM 1 del mes pasado) sin abrirlas una a una.
* Para extraer tendencias y patrones en diferentes fechas de producción y áreas de producción, apoyando las revisiones de gestión y la dirección de mejora continua.
* Para investigar un tema en el archivo de reuniones usando preguntas en lenguaje natural en cualquier idioma compatible.

## Requisitos previos

* Debe existir al menos una transcripción de reunión producida por Análisis de Reunión en el entorno DISS.
* El usuario debe tener acceso al archivo Overview Meeting.
* El usuario debe tener acceso de lectura a las reuniones incluidas en el análisis.

## Cómo usarla

{% stepper %}
{% step %}
### Navegar al archivo Overview Meeting

* Navegar al archivo **Overview Meeting** en DISS.

<figure><img src=".gitbook/assets/meeting-insight_overview-meeting-archive-page.png" alt="Página del archivo Overview Meeting"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Filtrar el archivo de reuniones

* Usar filtros de fecha o de nivel organizativo para aislar las reuniones relevantes para el ámbito de análisis.

<figure><img src=".gitbook/assets/meeting-insight_date-and-level-filters-on-the-archive.png" alt="Filtros de fecha y nivel en el archivo"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Seleccionar las reuniones a analizar

* Seleccionar múltiples reuniones usando las casillas a la izquierda de cada fila para definir el conjunto de datos de análisis.

<figure><img src=".gitbook/assets/meeting-insight_meetings-selected-via-checkboxes.png" alt="Reuniones seleccionadas mediante casillas"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lanzar Perspectivas de Reunión

* Hacer clic en **Resumir notas** para lanzar el Agente de Insight en las reuniones seleccionadas. El agente abre una ventana de diálogo donde se puede interactuar con el conjunto de datos combinado de todas las transcripciones seleccionadas.

<figure><img src=".gitbook/assets/meeting-insight_summarize-notes-button.png" alt="Botón Resumir notas"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Gestionar la selección activa

* Usar el panel lateral para ver o deseleccionar reuniones específicas sin cerrar el diálogo, manteniendo el control total sobre el ámbito de análisis.

<figure><img src=".gitbook/assets/meeting-insight_managing-the-active-selection-from-the-dialog.png" alt="Gestión de la selección activa desde el diálogo"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Extraer la lista de acciones

* Hacer clic en **Extraer lista de acciones** para agregar todas las acciones de las sesiones seleccionadas en una sola lista.

<figure><img src=".gitbook/assets/meeting-insight_action-items-list-aggregated-across-meetings.png" alt="Lista de acciones agregada de múltiples reuniones"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Hacer preguntas en lenguaje natural

* Hacer preguntas en lenguaje natural en el campo de entrada para localizar detalles operativos específicos — causas raíz, barreras recurrentes, responsables — en las transcripciones.

<figure><img src=".gitbook/assets/meeting-insight_natural-language-query-on-the-selected-meetings.png" alt="Consulta en lenguaje natural sobre las reuniones seleccionadas"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Exportar y marcar resultados

* Marcar como favoritas las consultas usadas frecuentemente para reutilización más rápida, y copiar los resúmenes generados o las listas de acciones a documentos externos para informes.

<figure><img src=".gitbook/assets/meeting-insight_bookmarking-a-query-and-exporting-the-results.png" alt="Marcando una consulta como favorita y exportando los resultados"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lectura del resultado

| Resultado                   | Descripción                                                                                                                                                        |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Lista de acciones           | Una lista consolidada y deduplicada de todas las acciones identificadas en las sesiones de reunión seleccionadas, con descripción, responsable inferido y reunión origen. |
| Respuesta en lenguaje natural | Una respuesta de IA sintetizada que se basa en el contenido transcrito completo de las reuniones seleccionadas, con referencias a la reunión y sesión origen.      |
| Consultas marcadas como favoritas | Consultas usadas frecuentemente guardadas y reutilizables desde el panel lateral, acelerando análisis recurrentes como verificaciones de tendencias semanales o revisiones de gestión. |

{% hint style="info" %}
Los resultados son orientativos. El líder de la reunión sigue siendo responsable de convertir los patrones recurrentes en contramedidas concretas a través de la función Acciones.
{% endhint %}

## Consejos y límites conocidos

{% hint style="info" %}
* La calidad de los insights escala con la calidad de las actas de Análisis de Reunión subyacentes: fomentar grabaciones limpias y la mención explícita de responsables y fechas durante las reuniones.
* Usar filtros antes de lanzar el agente — analizar un conjunto de datos enfocado (por ejemplo, un nivel SIM y un mes) produce insights más precisos que analizar todo el archivo.
* La participación de IA en tiempo real durante la reunión SIM en sí no forma parte de esta versión: Perspectivas de Reunión hoy opera sobre actas ya grabadas.
* Los insights son orientativos: el líder es responsable de traducir los patrones recurrentes en contramedidas concretas mediante Acciones o Katas.
{% endhint %}
