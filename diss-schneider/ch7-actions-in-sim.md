---
icon: list-check
---

# Actions in SIM

### Overview

The Actions feature in DISS is the structured way to record, assign, and track corrective and improvement activities directly from the SIM Boards. Two complementary use cases are documented here: **Create Action** — to register a brand-new action with full SIM context — and **Edit Action** — to keep an existing action up to date while the team resolves it during the daily SIM routine.

## When to use it

* Open a **Create Action** during a SIM meeting whenever a problem or opportunity is identified on the line: a Safety / Quality / Delivery / Maintenance / Production / Engineering issue with a clear owner and due date
* Open an **Edit Action** between SIM meetings to keep an action up to date: status progression, refined description, new attachments, solutions captured, or notes added to the Activity Log
* Use Actions in SIM to ensure every problem surfaced on a SIM Board is converted into a traceable, assignable activity rather than remaining a verbal commitment

## Prerequisites

* The user must have access to the SIM Boards on which Actions are enabled
* Action categories, production areas, and lines must be configured in **Plant Configuration** — they populate the Category, Module, and Line fields in the Create Action form
* Owner or Team must exist in DISS to be assignable to the action

## How to use it — Create Action

{% stepper %}
{% step %}
### Open the Create Action form

From the SIM Board, open the **Create Action** form.

<figure><img src="../.gitbook/assets/create-action_entry-point-on-the-sim-board.png" alt="Create Action entry point on the SIM Board"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set the SIM context

Set the SIM context: **Category** (Safety, Quality, Delivery, Maintenance, Production, Engineering), **Module** (pre-filled with the Production Area from the originating board), **Line**. Source SIM level and Target SIM level are auto-selected from the originating SIM Board; verify them before saving as the Source SIM level becomes immutable once saved.

<figure><img src="../.gitbook/assets/create-action_sim-context-bar-category.png" alt="Create Action SIM context bar with Category"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Write the Title

Write a **Title** that identifies the problem (max 500 characters).

<figure><img src="../.gitbook/assets/create-action_title-field.png" alt="Create Action Title field"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set the Status

Leave **Status** as "New" unless your local SIM process requires a different starting status.

<figure><img src="../.gitbook/assets/create-action_status-dropdown.png" alt="Create Action Status dropdown"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Write the Description

Write the **Description**. Use bold, italic, and lists for readability. Optionally click **AI Enhance** to improve clarity; the quality indicator gives real-time feedback as you type.

<figure><img src="../.gitbook/assets/create-action_description-with-ai-enhance-and-quality-indica.png" alt="Description with AI Enhance and quality indicator"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set the Due Date

Pick a **Due Date** — by default today + 7 days; past dates are not allowed.

<figure><img src="../.gitbook/assets/create-action_due-date-picker.png" alt="Create Action Due Date picker"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set Priority and Severity

Set **Priority** (Trivial / Minor / Major / Critical / Blocker) and **Severity**.

<figure><img src="../.gitbook/assets/create-action_priority-and-severity-dropdowns.png" alt="Priority and Severity dropdowns"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Assign the Raiser, Team, and Owner

Confirm the **Raiser** (pre-filled with the current user; change only when registering on behalf of another). Assign responsibility: at least one between **Team** and **Owner** must be set so the action has a clear accountable party on the SIM Board.

<figure><img src="../.gitbook/assets/create-action_team-and-owner-assignment.png" alt="Team and Owner assignment"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Save the Action

Click **Save Action**. The green button activates only when all required fields are populated. Once saved, the action is visible on the SIM Board.

<figure><img src="../.gitbook/assets/create-action_save-action-button-active-and-action-visible-o.png" alt="Save Action button active and action visible on SIM Board"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## How to use it — Edit Action

Edit Action is **auto-saving**: each field is committed individually when you leave the field. There is no global Save button — the header displays "All changes saved" as confirmation. This behaviour allows updates to be made quickly during the SIM stand-up without interrupting the meeting rhythm.

{% stepper %}
{% step %}
### Open the action from the SIM Board

From the SIM Board, open the action you want to update.

<figure><img src="../.gitbook/assets/edit-action_opening-an-action-from-the-sim-board.png" alt="Opening an action from the SIM Board"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Update the Entry Panel fields

Update the editable fields in the Entry Panel: **Title, Status, Description** (with AI Enhance and quality indicator), **Due Date, Priority, Severity, Raiser, Team, Owner, Attachments**.

<figure><img src="../.gitbook/assets/edit-action_entry-panel-with-all-editable-fields.png" alt="Entry Panel with all editable fields"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Escalate to a higher SIM level if needed

Change the **Target SIM level** in the context bar if the action needs to be escalated (it is the only context-bar field that remains editable after creation).

<figure><img src="../.gitbook/assets/edit-action_target-tier-dropdown-in-the-context-bar.png" alt="Target SIM level dropdown in the context bar"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Add or review Solutions & Proposals

In the **Solutions & Proposals** panel, type or paste the proposed solution, or click **AI Suggest** to auto-generate solution proposals scored by relevance. The proposals are extracted from the documents uploaded to the DeepFind Knowledge Source.

<figure><img src="../.gitbook/assets/edit-action_solutions-&-proposals-with-ai-suggest.png" alt="Solutions & Proposals with AI Suggest"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Add notes to the Activity Log

Add notes to the **Activity Log** at the bottom of the panel; attach files via the paperclip icon if needed. The Activity Log is the full history of the action on the SIM Board.

<figure><img src="../.gitbook/assets/edit-action_activity-log-with-note-input-and-paperclip.png" alt="Activity Log with note input and paperclip"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set the action to Done

Set the **Status** to "Done" only when the action is genuinely complete: "Done" locks the entire record.

<figure><img src="../.gitbook/assets/edit-action_status-set-to-done-(locked-record).png" alt="Status set to Done — locked record"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Reading the result

* **Quality indicator** on the Description — Poor / Fair / Good / Excellent — signals whether the text contains enough information to be acted on
* **AI Enhance** rewrites the text for professional clarity; always review the result before saving
* **AI Suggest** in Solutions ranks proposals by relevance percentage to the Description content
* Email notifications are sent on status change, new Team/Owner assignment, 48-hour due-date warning, and overdue actions

## Tips & known limits

{% hint style="info" %}
* Do not set Status to "Done" until the action is genuinely complete: it cannot be edited after that
* If both Team and Owner are cleared, saving fails — always keep at least one assigned
* Auto-save reverts the field on error: check the network connection if you see a save error message
* AI Enhance and AI Suggest are assistive: the responsible Owner remains accountable for the final wording and the chosen solution
* Escalation across SIM levels is performed by changing the Target SIM level, not by creating a new action — this preserves the Activity Log history of the original problem
{% endhint %}
