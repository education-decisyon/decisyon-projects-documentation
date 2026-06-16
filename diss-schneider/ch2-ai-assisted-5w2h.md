---
icon: star-half-stroke
---

# AI-Assisted 5W2H

### Overview

AI-Assisted 5W2H is a quality assessment widget that evaluates how complete and clear a Kata problem statement is. It scores the text written by the user in the Current State and Target State fields against the 5W2H framework — Who, What, Why, When, Where, How, How Many — and returns an overall quality score and per-dimension feedback. The objective is to standardise quality checks across teams and plants, removing inconsistent and subjective reviews.

## When to use it

* While drafting the Current State or Target State of a new Kata, to make sure the problem statement is precise enough to be actionable
* During a coaching session, to support the conversation with evidence taken directly from the user's own text
* Over time, to track how the quality of problem statements evolves across teams via a stable numeric score

## Prerequisites

* The 5W2H widget must be enabled on the Kata fields where it should run (typically Current State and Target State)
* The user must have permission to edit the Kata in question

## How to use it

{% stepper %}
{% step %}
### Navigate to Kata QRCI

Navigate to **Digitized Idea & SIM System → Kata QRCI**. The dashboard lists all existing Katas, filterable by date range, Status, and KPI. Click **Add** (top-right) to open the new Kata creation form.

<figure><img src="../.gitbook/assets/kata-qrci_dashboard-with-kata-list-and-add-button-highlighte.png" alt="Kata QRCI dashboard with Add button highlighted"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Fill in the Kata header

In the Add form, set the context fields: **Production Area** and **Line** (from the plant hierarchy), **Title** (a concise problem statement), **Leader** and **Coach** (both required), **Source** (the origin category of the problem — e.g. Downtime, Efficiency, Maintenance issues, Check Do check non-conformance, High lead time, Layered Process audit non-conformance), and **KPI** (e.g. OEE). Creation Date is pre-filled with today.

<figure><img src="../.gitbook/assets/kata-qrci_add-form-with-header-fields-filled-in:-production-.png" alt="Kata QRCI Add form with header fields filled in"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Write the Current Status (5W2H) and Target

In the **Current Status** and **Target (5W2H)** fields, describe the current situation and the desired end state clearly and measurably following the 5W2H framework: Who, What, Why, When, Where, How, How Many.

<figure><img src="../.gitbook/assets/[-screenshot_5w2h_kata-form-with-current-state---target-stat.png" alt="Kata form with Current State and Target State fields"><figcaption></figcaption></figure>

As you type, the inline badge in the widget shows the current quality score and the character count. Click the inline badge to open the detailed popup. Review the circular score, the qualitative label, and the **Focus on:** priority area suggested by the AI. Add missing information in your text; the score updates as you save the field.

<figure><img src="../.gitbook/assets/5w2h_inline-quality-badge-updating-live-as-the-user-types.png" alt="Inline quality badge updating live as the user types"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/5w2h_clicking-the-badge-opens-the-detailed-popup.png" alt="Clicking the badge opens the detailed popup"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/5w2h_detailed-popup-with-circular-score-and-focus-on-area.png" alt="Detailed popup with circular score and Focus on area"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/5w2h_score-recalculated-after-adding-missing-information.png" alt="Score recalculated after adding missing information"><figcaption></figcaption></figure>

Click **Save** to create the Kata.

<figure><img src="../.gitbook/assets/kata-qrci_add-form-with-current-status-and-target-fields-(5w.png" alt="Add form with Current Status and Target fields filled in"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Open the Kata to activate the 5W2H widget

The new Kata appears in the Kata QRCI list. Open it: the AI-Assisted 5W2H widget is now active on the Current State and Target State fields and begins evaluating the text you entered.

<figure><img src="../.gitbook/assets/kata-qrci_newly-created-kata-visible-in-the-list,-ready-to-o.png" alt="Newly created Kata visible in the list, ready to open"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Reading the result

### The 7 dimensions

Every problem statement is evaluated against the same fixed set of dimensions, in this order: **Who, What, Why, When, Where, How, How Many**.

### Per-dimension score

Each dimension receives a traffic-light colour and a numeric score based on how completely and specifically it is addressed in the text.

### Overall quality score

The total is the sum of the 7 per-dimension scores (maximum 14), expressed as a percentage of 14 to give a 0–100 quality score.

### Summary table

For every dimension the widget displays four columns:

| Column | Description |
|--------|-------------|
| Question | The 5W2H dimension being evaluated |
| Evaluation | The per-dimension score and traffic-light colour |
| Excerpt | The portion of your text that the AI used to evaluate the dimension |
| Suggestion | What to add or clarify (shown when the dimension is missing or vague) |

## Tips & known limits

{% hint style="info" %}
* The user retains full control: AI suggestions are advisory — the final text is always written and saved by the user
* The score is computed against the text in the current field — write the Current State and the Target State independently to get reliable per-field feedback
* The widget rewards specificity: dates, names, lines, KPIs, and measurable quantities lift the score quickly
* Translation is a presentation feature: the score is calculated on the original text
* Two problem statements with the same overall score can have very different per-dimension profiles — use the summary table, not just the overall percentage, to decide what to improve
* AI-Assisted 5W2H is a guidance tool: a sustained low score is a signal that the team needs coaching on problem framing
{% endhint %}
