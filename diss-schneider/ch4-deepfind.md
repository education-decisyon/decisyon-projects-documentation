# 4  DEEPFIND

## 4.1  What it is

![DeepFind is an AI chatbot embedded in DISS that lets users query a configured Knowledge Source — a repository of plant manuals, procedures, FAQs, policies, reports — using natural language. DeepFind scans the documents that have been uploaded and synthesises an answer grounded on their content. Multiple documents can be attached to the same conversation to provide a richer context for the AI.](.gitbook/assets/deepfind-is-an-ai-chatbot-embedded-in-diss-that-lets-users-q.png)

## 4.2  When to use it

Use DeepFind to retrieve operational information without searching through documents page by page. Typical examples:
Looking up the procedure for a specific intervention on a piece of equipment
Verifying the prerequisites or steps of a quality / safety policy
Identifying an error code that appeared on a machine and looking up the recommended troubleshooting and corrective actions
Finding the right paragraph in a long technical manual during a Kata investigation

## 4.3  Prerequisites

A Knowledge Source must be configured for your plant in DISS
The relevant documents (manuals, procedures, FAQs, error-code references) must have been uploaded to the Knowledge Source

![DeepFind must be explicitly enabled on that Knowledge Source](.gitbook/assets/deepfind-must-be-explicitly-enabled-on-that-knowledge-source.png)

## 4.4  How to use it

### Step 1 — Upload documents to the Knowledge Source

This step is performed by a user with the Knowledge Source administrator scope and must be completed before end users can query DeepFind.

![DISS — user profile details with Knowledge Source administrator scope highlighted](.gitbook/assets/diss_user-profile-details-with-knowledge-source-administrato.png)

- Click your user avatar in the top-right corner of the application and select Knowledge Sources from the dropdown menu.

![Knowledge Sources — profile dropdown showing the Knowledge Sources option](.gitbook/assets/knowledge-sources_profile-dropdown-showing-the-knowledge-sou.png)

- In the left panel, click + to open the Create knowledge source dialog. Enter a descriptive name (for example: DISS User Manual / Func Spec) and click Create. The new Knowledge Source appears in the left panel as a named container. To use an existing one, simply select it from the list.
- With the Knowledge Source selected, go to the Documents tab and click Import File. Select the document to upload (PDF or compatible format) and confirm. Repeat for each additional file. Uploaded documents appear in the list with Enabled or Disabled status.

![Knowledge Sources — Documents tab with Import File button and uploaded document list](.gitbook/assets/knowledge-sources_documents-tab-with-import-file-button-and-.png)

- In the Permissions tab, assign the organisations and user groups that are allowed to query this Knowledge Source.

![Knowledge Sources — Permissions tab with organisation and group configured](.gitbook/assets/knowledge-sources_permissions-tab-with-organisation-and-grou.png)

- In the AI Agents tab, enable the DeepFind AI Assistant toggle to connect this Knowledge Source to the DeepFind feature. Enable Fix Finder too if applicable.

![Knowledge Sources — AI Agents tab with DeepFind AI Assistant enabled](.gitbook/assets/knowledge-sources_ai-agents-tab-with-deepfind-ai-assistant-e.png)

- Once configured, the knowledge base is immediately available to all users in the assigned organisations.

### Step 2 — Open DeepFind

Locate the DeepFind Assistant icon in the DISS toolbar.

![DeepFind — Assistant icon in the toolbar](.gitbook/assets/deepfind_assistant-icon-in-the-toolbar.png)

### Step 3 — Open the chat interface

Click the icon to open the chat interface.

![DeepFind — chat interface opened (empty state)](.gitbook/assets/deepfind_chat-interface-opened-(empty-state).png)

### Step 4 — Ask a question

Type your question in natural language — full sentences work better than keyword searches. For troubleshooting, include the error code and a short description of the symptom.

![DeepFind — typing a natural-language question (with error code example)](.gitbook/assets/deepfind_typing-a-natural-language-question-(with-error-code.png)

### Step 5 — Read the answer and follow up

Read the synthesised answer. DeepFind cites the source document and section at the bottom of each response, so you can verify where the information comes from. If needed, ask a follow-up question to refine or expand the answer.

![DeepFind — synthesised answer and follow-up turn](.gitbook/assets/deepfind_synthesised-answer-and-follow-up-turn.png)

## 4.5  Reading the result

![DeepFind synthesises one answer based on the most relevant passages it found in the configured Knowledge Source and in the documents attached to the conversation. The answer respects the access policies of the underlying documents: a user only sees information from documents they are allowed to access.](.gitbook/assets/deepfind-synthesises-one-answer-based-on-the-most-relevant-p.png)

When DeepFind cannot answer based on the available material, it returns the message: "I'm sorry, but I can't help with that because it's outside the scope of my knowledge." This means that no relevant document was found, not that the topic does not exist.

## 4.6  Tips & known limits

Ask one question at a time — compound questions tend to be answered partially
If the answer is incomplete, rephrase with different keywords or be more specific about the equipment / process / error code
If the question is in scope but no answer is found, ask your DISS administrator to verify that the relevant document is uploaded and DeepFind is enabled on that Knowledge Source

![DeepFind does not invent content: it only references material present in the configured Knowledge Source or in the attached documents](.gitbook/assets/deepfind-does-not-invent-content:-it-only-references-materia.png)
