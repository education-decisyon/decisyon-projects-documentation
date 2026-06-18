---
icon: clock-rotate-left
---

# 3. Historical Lookup

### Overview

**Historical Lookup** es una función de IA que, partiendo del Kata QRCI en el que se está trabajando, busca los Katas cerrados del mismo centro y devuelve los más similares. Para cada Kata histórico el usuario puede revisar la explicación de IA sobre la coincidencia e importar — selectivamente — las acciones que se utilizaron para resolver el problema pasado, acelerando la respuesta ante problemas recurrentes.

<figure><img src=".gitbook/assets/historical-lookup_ai-analysis-accordion-expanded.png" alt=""><figcaption></figcaption></figure>

## Cuándo usarla

* Cuando un problema en planta resulta familiar pero el equipo no recuerda cuándo, dónde y cómo se resolvió antes.
* Antes de guardar un nuevo Kata, para comprobar si el mismo problema ya se ha abordado y evitar duplicar esfuerzos.
* Durante el análisis de causa raíz, para leer cómo los compañeros formularon el Estado Actual y el Estado Objetivo en un caso comparable.

## Requisitos previos

* El Kata actual debe tener un Centro definido: Historical Lookup solo se activa cuando el Centro está configurado.
* Debe existir al menos un Kata con estado **Cerrado** en el ámbito de búsqueda para que la IA encuentre alguna coincidencia.
* El usuario debe tener acceso de lectura a los Katas históricos en el ámbito de búsqueda.

## Cómo usarla

{% stepper %}
{% step %}
### Abrir el Panel Kata

* Abrir el **Panel Kata** en DISS.

<figure><img src=".gitbook/assets/historical-lookup_kata-dashboard-with-the-ai-tools-column-visible.png" alt="Panel Kata con la columna de herramientas de IA visible"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Iniciar Historical Lookup

* En la columna **Kata**, hacer clic en el **icono de similitud Kata** junto al Kata Abierto en el que se está trabajando.

<figure><img src=".gitbook/assets/historical-lookup_icon-highlighted-on-a-kata-row.png" alt="Icono de similitud Kata destacado en una fila del Kata"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Esperar a que finalice la búsqueda de IA

* El modal **AI Historical Lookup** se abre y la búsqueda comienza automáticamente — no se requiere ninguna entrada adicional. Esperar a que el mensaje de carga ("Cargando Katas similares…") finalice.

<figure><img src=".gitbook/assets/historical-lookup_modal-in-loading-state.png" alt="Modal Historical Lookup en estado de carga"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Revisar los Katas similares

* Revisar los hasta 5 Katas cerrados devueltos, ordenados por puntuación de similitud descendente.

<figure><img src=".gitbook/assets/historical-lookup_list-of-matches-with-similarity-scores.png" alt="Lista de coincidencias con puntuaciones de similitud"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Analizar cada coincidencia en detalle

* Para cada coincidencia, expandir el acordeón **Análisis de IA** para leer "**Por qué coincide**" y "**Diferencias a considerar**".

<figure><img src=".gitbook/assets/historical-lookup_ai-analysis-accordion-expanded.png" alt="Acordeón de Análisis de IA expandido"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Copia selectiva de acciones

Cada coincidencia histórica tiene un selector **Acciones reutilizables**. Cuando se expande, se cargan las acciones de ese Kata y aparece una casilla junto a cada acción. Se puede:

* Seleccionar acciones individuales una a una;
* Usar **Seleccionar todo / Deseleccionar todo** dentro de un Kata histórico;
* Combinar selecciones de múltiples Katas en la misma sesión — el recuento total siempre es visible.

Cuando al menos una acción está seleccionada, el botón **Importar N acciones** aparece en la parte inferior. Hacer clic en él para copiar las acciones seleccionadas al Kata actual. Para cada acción importada:

* Se copian el **Título** y la **descripción** del origen;
* El estado se restablece a Abierto;
* La fecha límite por defecto es hoy + 7 días; el nuevo responsable establece una fecha nueva.

Al completarse, el modal se cierra automáticamente, aparece un mensaje de confirmación y la tabla de Acciones del Kata actual se actualiza para mostrar los nuevos registros.

{% stepper %}
{% step %}
### Cargar acciones históricas

* En una de las coincidencias, hacer clic en **Acciones reutilizables** para cargar las acciones históricas de ese Kata.

<figure><img src=".gitbook/assets/selective-action-copy_view-actions-toggle-expanded-for-a-match.png" alt="Selector de acciones reutilizables expandido para una coincidencia"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Seleccionar las acciones a importar

* Usar las casillas para seleccionar acciones individuales, o usar **Seleccionar todo / Deseleccionar todo** para actuar sobre todo el Kata.

<figure><img src=".gitbook/assets/Selective Action Copy — checkboxes and Select All - Deselect All controls.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Combinar selecciones de múltiples Katas

* Opcionalmente repetir para otras coincidencias: la selección persiste entre múltiples Katas en la misma sesión.

<figure><img src=".gitbook/assets/selective-action-copy_multi-kata-selection-with-total-counter-visible.png" alt="Selección de múltiples Katas con contador total visible"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Importar las acciones seleccionadas

* Hacer clic en **Importar N acciones** en la parte inferior del modal.

<figure><img src=".gitbook/assets/Selective Action Copy — Import N Actions button.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirmar y verificar las acciones importadas

* El modal se cierra, aparece una confirmación y la tabla de Acciones del Kata actual se actualiza con los nuevos registros (Estado = Abierto, Fecha límite = Fecha actual).

<figure><img src=".gitbook/assets/selective-action-copy_current-kata-actions-table-refreshed-with-imported-records.png" alt="Tabla de Acciones del Kata actual actualizada con los registros importados"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lectura del resultado

| Campo                    | Descripción                                                                                                                                                                                          |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Puntuación de similitud  | Un porcentaje (0–100) que indica cuán estrechamente coincide el Kata cerrado con el abierto. Puntuaciones superiores a 70 indican una fuerte superposición temática; puntuaciones inferiores a 40 son coincidencias débiles mostradas para completar. |
| Por qué coincide         | Una explicación concisa generada por IA de los elementos compartidos entre los dos Katas.                                                                                                            |
| Diferencias a considerar | Un breve resumen de lo que distingue el caso histórico del actual.                                                                                                                                   |
| Acciones reutilizables   | La lista completa de acciones del Kata histórico, listas para importación selectiva.                                                                                                                 |

## Consejos y límites conocidos

{% hint style="info" %}
* Por defecto, Historical Lookup busca solo dentro del centro actual. Cuando el ámbito multi-planta está habilitado, el centro de origen se etiqueta claramente en cada resultado.
* Solo se consideran los Katas **Cerrados**; los Katas en curso se excluyen.
* Los Katas idénticos o casi idénticos no se ocultan — aparecen con una similitud muy alta para que puedas decidir si importar sus acciones.
* Las acciones importadas siempre comienzan de nuevo (Estado = Abierto, Fecha límite = por defecto hoy + 7 días): el nuevo responsable asume la propiedad del plazo.
* Los filtros de Área, Línea, Origen y KPI NO son filtros estrictos — la IA los usa como contexto semántico, lo que significa que una coincidencia relevante de una Línea diferente puede seguir siendo propuesta.
{% endhint %}
