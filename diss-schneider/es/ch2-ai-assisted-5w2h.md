---
icon: star-half-stroke
---

# 2. AI-Assisted 5W2H

### Descripción general

**AI-Assisted 5W2H** es un widget de evaluación de calidad que analiza qué tan completo y claro es el enunciado de un problema Kata. Puntúa el texto escrito por el usuario en los campos Estado Actual y Estado Objetivo según el marco 5W2H — **Quién, Qué, Por qué, Cuándo, Dónde, Cómo, Cuántos** — y devuelve una puntuación global de calidad y retroalimentación por dimensión. El objetivo es estandarizar las verificaciones de calidad entre equipos y plantas, eliminando revisiones inconsistentes y subjetivas.

<figure><img src=".gitbook/assets/5W2H Cover - Welcome page.png" alt=""><figcaption></figcaption></figure>

## Cuándo usarla

* Al redactar el **Estado Actual** o el **Estado Objetivo** de un nuevo Kata, para asegurarse de que el enunciado del problema sea suficientemente preciso y accionable.
* Durante una sesión de coaching, para apoyar la conversación con evidencia tomada directamente del texto del usuario.
* A lo largo del tiempo, para hacer seguimiento de cómo evoluciona la calidad de los enunciados de problema entre equipos mediante una puntuación numérica estable.

## Requisitos previos

* El widget **5W2H** debe estar habilitado en los campos Kata donde debe ejecutarse (generalmente Estado Actual y Estado Objetivo).
* El usuario debe tener permiso para editar el Kata en cuestión.

## Cómo usarla

{% stepper %}
{% step %}
### Navegar a Kata QRCI

* Navegar a **Digitized Idea & SIM System → Kata QRCI**. El panel muestra todos los Katas existentes, filtrables por rango de fechas, Estado y KPI. Hacer clic en **Añadir** (arriba a la derecha) para abrir el formulario de creación de nuevo Kata.

<figure><img src=".gitbook/assets/kata-qrci_dashboard-with-kata-list-and-add-button-highlighted.png" alt="Panel Kata QRCI con el botón Añadir destacado"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Completar el encabezado del Kata

En el formulario de añadir, configurar los campos de contexto:

* **Área de producción** y **Línea** (de la jerarquía de planta);
* **Título** (un enunciado conciso del problema);
* **Líder** y **Coach** (ambos obligatorios);
* **Origen** (la categoría de origen del problema — p. ej. Tiempo de parada, Eficiencia, Problemas de mantenimiento) y **KPI** (p. ej. OEE);
* **Fecha de creación** se completa automáticamente con la fecha actual.

<figure><img src=".gitbook/assets/Kata QRCI — Add form with header fields filled in.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Escribir el Estado Actual (5W2H) y el Objetivo

* En los campos **Estado Actual** y **Objetivo (5W2H)**, describir la situación actual y el estado final deseado de forma clara y medible siguiendo el marco 5W2H: **Quién, Qué, Por qué, Cuándo, Dónde, Cómo, Cuántos.**

<figure><img src=".gitbook/assets/5w2h_kata-form-with-current-state-target-state-fields.png" alt="Formulario Kata con campos Estado Actual y Estado Objetivo"><figcaption></figcaption></figure>

* Al escribir, el indicador en línea del widget muestra la puntuación de calidad actual y el recuento de caracteres.

<figure><img src=".gitbook/assets/5w2h_inline-quality-badge-updating-live-as-the-user-types.png" alt="Indicador de calidad en línea actualizándose en tiempo real" width="473"><figcaption></figcaption></figure>

* Hacer clic en el indicador en línea para abrir el popup detallado.

<figure><img src=".gitbook/assets/5w2h_clicking-the-badge-opens-the-detailed-popup.png" alt="Al hacer clic en el indicador se abre el popup detallado" width="563"><figcaption></figcaption></figure>

* Revisar la puntuación circular, la etiqueta cualitativa y el área de **Enfoque en:** sugerida por la IA.

<figure><img src=".gitbook/assets/5w2h_detailed-popup-with-circular-score-and-focus-on-area.png" alt="Popup detallado con puntuación circular y área de enfoque" width="563"><figcaption></figcaption></figure>

* Añadir la información faltante en el texto; la puntuación se actualiza al guardar el campo.

<figure><img src=".gitbook/assets/5w2h_score-recalculated-after-adding-missing-information.png" alt="Puntuación recalculada tras añadir información faltante"><figcaption></figcaption></figure>

* Hacer clic en **Guardar** para crear el Kata.

<figure><img src=".gitbook/assets/kata-qrci_add-form-with-current-status-5w2h-and-target-fields-filled-in.png" alt="Formulario con campos Estado Actual y Objetivo (5W2H) completados"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Abrir el Kata para activar el widget 5W2H

* El nuevo Kata aparece en la lista **Kata QRCI**. Abrirlo: el widget **AI-Assisted 5W2H** está ahora activo en los campos Estado Actual y Estado Objetivo y comienza a evaluar el texto introducido.

<figure><img src=".gitbook/assets/kata-qrci_newly-created-kata-visible-in-the-list-ready-to-open.png" alt="Nuevo Kata visible en la lista, listo para abrir"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lectura del resultado

### Las 7 dimensiones

Cada enunciado de problema se evalúa según el mismo conjunto fijo de dimensiones, en este orden: **Quién, Qué, Por qué, Cuándo, Dónde, Cómo, Cuántos**.

### Puntuación por dimensión

Cada dimensión recibe un color semáforo y una puntuación numérica en función de lo completa y específicamente que se aborda en el texto.

### Puntuación global de calidad

El total es la suma de las 7 puntuaciones por dimensión (máximo 14), expresada como porcentaje de 14 para obtener una puntuación de calidad de 0 a 100.

### Tabla resumen

Para cada dimensión el widget muestra cuatro columnas:

| Columna     | Descripción                                                            |
| ----------- | ---------------------------------------------------------------------- |
| Pregunta    | La dimensión 5W2H que se está evaluando                                |
| Evaluación  | La puntuación por dimensión y el color semáforo                        |
| Fragmento   | La parte del texto que la IA utilizó para evaluar la dimensión         |
| Sugerencia  | Qué añadir o aclarar (se muestra cuando la dimensión falta o es vaga)  |

## Consejos y límites conocidos

{% hint style="info" %}
* El usuario mantiene el control total: las sugerencias de IA son orientativas — el texto final siempre lo escribe y guarda el usuario
* La puntuación se calcula sobre el texto del campo actual — escribir el Estado Actual y el Estado Objetivo de forma independiente para obtener retroalimentación fiable por campo
* El widget recompensa la especificidad: fechas, nombres, líneas, KPIs y cantidades medibles elevan la puntuación rápidamente
* La traducción es una función de presentación: la puntuación se calcula sobre el texto original
* Dos enunciados de problema con la misma puntuación global pueden tener perfiles por dimensión muy diferentes — usar la tabla resumen, no solo el porcentaje global, para decidir qué mejorar
* AI-Assisted 5W2H es una herramienta de orientación: una puntuación persistentemente baja es una señal de que el equipo necesita coaching sobre cómo formular problemas
{% endhint %}
