---
icon: magnifying-glass
---

# 4. DeepFind

### Overview

DeepFind is an AI chatbot embedded in DISS that lets users query a configured Knowledge Source — a repository of plant manuals, procedures, FAQs, policies, reports — using natural language. DeepFind scans the documents that have been uploaded and synthesises an answer grounded on their content. Multiple documents can be attached to the same conversation to provide a richer context for the AI.

<figure><img src=".gitbook/assets/DeepFind-Cover Welcome page.png" alt=""><figcaption></figcaption></figure>

## When to use it

* Looking up the procedure for a specific intervention on a piece of equipment
* Verifying the prerequisites or steps of a quality or safety policy
* Identifying an error code that appeared on a machine and finding the recommended troubleshooting and corrective actions
* Finding the right paragraph in a long technical manual during a Kata investigation

## Prerequisites

* A Knowledge Source must be configured for your plant in DISS
* The relevant documents (manuals, procedures, FAQs, error-code references) must have been uploaded to the Knowledge Source
* DeepFind must be explicitly enabled on that Knowledge Source

{% hint style="info" %}
If DeepFind is not visible in your DISS toolbar, contact your DISS administrator to verify that a Knowledge Source with DeepFind enabled has been configured for your plant.
{% endhint %}

## How to use it

{% stepper %}
{% step %}
### Configure the Knowledge Source

This step is performed by a user with the **Knowledge Source administrator** scope and must be completed before end users can query DeepFind.

<figure><img src=".gitbook/assets/diss_user-profile-details-with-knowledge-source-administrator-scope-highlighted.png" alt="User profile with Knowledge Source administrator scope highlighted"><figcaption></figcaption></figure>

Click your user avatar in the top-right corner and select **Knowledge Sources** from the dropdown menu. In the left panel, click **+** to open the Create knowledge source dialog. Enter a descriptive name and click **Create**.

With the Knowledge Source selected, go to the **Documents** tab and click **Import File** to upload the relevant documents (PDF or compatible format). Repeat for each additional file.

<figure><img src=".gitbook/assets/knowledge-sources_documents-tab-with-import-file-button-and-uploaded-document-list.png" alt="Documents tab with Import File button and uploaded document list"><figcaption></figcaption></figure>

In the **Permissions** tab, assign the organisations and user groups allowed to query this Knowledge Source.

<figure><img src=".gitbook/assets/knowledge-sources_permissions-tab-with-organisation-and-group-configured.png" alt="Permissions tab with organisation and group configured"><figcaption></figcaption></figure>

In the **AI Agents** tab, enable the **DeepFind AI Assistant** toggle to connect this Knowledge Source to DeepFind.

<figure><img src=".gitbook/assets/knowledge-sources_ai-agents-tab-with-deepfind-ai-assistant-enabled.png" alt="AI Agents tab with DeepFind AI Assistant enabled"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Open DeepFind

Locate the **DeepFind Assistant** icon in the DISS toolbar and click it to open the chat interface.

<figure><img src=".gitbook/assets/deepfind_assistant-icon-in-the-toolbar.png" alt="DeepFind Assistant icon in the toolbar"><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/deepfind_chat-interface-opened-empty-state.png" alt="DeepFind chat interface opened (empty state)"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Ask a question

Type your question in natural language — full sentences work better than keyword searches. For troubleshooting, include the error code and a short description of the symptom.

<figure><img src=".gitbook/assets/deepfind_typing-a-natural-language-question-with-error-code-example.png" alt="Typing a natural-language question with error code example"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Read the answer and follow up

Read the synthesised answer. DeepFind cites the source document and section at the bottom of each response, so you can verify where the information comes from. If needed, ask a follow-up question to refine or expand the answer.

<figure><img src=".gitbook/assets/deepfind_synthesised-answer-and-follow-up-turn.png" alt="Synthesised answer and follow-up turn"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Reading the result

DeepFind synthesises one answer based on the most relevant passages found in the configured Knowledge Source and in any documents attached to the conversation. The answer respects the access policies of the underlying documents: a user only sees information from documents they are allowed to access.

When DeepFind cannot answer based on the available material, it returns: _"I'm sorry, but I can't help with that because it's outside the scope of my knowledge."_ This means that no relevant document was found, not that the topic does not exist.

## Tips & known limits

{% hint style="info" %}
* Ask one question at a time — compound questions tend to be answered partially
* If the answer is incomplete, rephrase with different keywords or be more specific about the equipment, process, or error code
* If the question is in scope but no answer is found, ask your DISS administrator to verify that the relevant document is uploaded and DeepFind is enabled on that Knowledge Source
* DeepFind does not invent content: it only references material present in the configured Knowledge Source or in the attached documents
{% endhint %}
