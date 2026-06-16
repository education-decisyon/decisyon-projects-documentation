# 3  HISTORICAL LOOKUP

## 3.1  What it is

![Historical Lookup is an AI feature that, starting from the Kata QRCI you are currently working on, searches the closed Katas of the same Plant and returns the most similar ones. For each historical Kata the user can review the AI explanation of the match and import — selectively — the actions that were used to solve the past problem, accelerating the response to recurring issues.](.gitbook/assets/historical-lookup-is-an-ai-feature-that,-starting-from-the-k.png)

## 3.2  When to use it

Whenever a problem on the shop floor feels familiar but the team cannot remember when, where, and how it was solved before
Before saving a new Kata, to check whether the same problem has already been tackled and avoid duplicating effort
During root-cause analysis, to read how peers formulated the Current State and the Target State for a comparable case

## 3.3  Prerequisites

The current Kata must have a Plant defined: Historical Lookup is enabled only when the Plant is set
There must be at least one Kata with status Closed in the search perimeter for the AI to find any match
The user must have read access to the historical Katas in the search perimeter

## 3.4  How to use it

### Step 1 — Open the Kata Dashboard

Open the Kata Dashboard in DISS.

![Historical Lookup — Kata Dashboard with the AI Tools column visible](.gitbook/assets/historical-lookup_kata-dashboard-with-the-ai-tools-column-vi.png)

### Step 2 — Launch the Historical Lookup

In the AI Tools column, click the Kata Similarity icon next to the Open Kata you are working on, in this example the Kata “Station 3 Scrap Rate Exceeding Threshold — OEE Loss on Line AI 1” previously created that has no actions anymore.

![Historical Lookup — Icon highlighted on a Kata row](.gitbook/assets/historical-lookup_icon-highlighted-on-a-kata-row.png)

### Step 3 — Wait for the AI search to complete

The AI Historical Lookup modal opens and the search starts automatically — no additional input is required. Wait for the loading message ("AI-Powered Semantic Search…") to complete.

![Historical Lookup — modal in loading state](.gitbook/assets/historical-lookup_modal-in-loading-state.png)

### Step 4 — Review the similar Katas

Review the up-to-5 closed Katas returned, sorted by similarity score descending.

![Historical Lookup — list of matches with similarity scores](.gitbook/assets/historical-lookup_list-of-matches-with-similarity-scores.png)

### Step 5 — Analyse each match in detail

For each match, expand the AI Analysis accordion to read "Why it matches" and "Key Differences".

![Historical Lookup — AI Analysis accordion expanded](.gitbook/assets/historical-lookup_ai-analysis-accordion-expanded.png)

## 3.5  Selective Action Copy

Each historical match has a View actions toggle. When expanded, the actions of that Kata are loaded from the database and a checkbox appears next to each action. You can:
Select individual actions one by one
Use Select All / Deselect All inside one historical Kata to act on all its actions at once
Combine actions from multiple historical Katas in the same modal session — the total count is always visible
When at least one action is selected, the "Import N Actions" button appears at the bottom. Click it to copy the selected actions into the current Kata. For each imported action:
Title, description, and owner are copied from the source
Status is reset to Open
Due date is cleared (set to empty) — the new owner will pick a fresh deadline
On success, the modal closes automatically, a confirmation message appears, and the Actions table of the current Kata refreshes to show the new records.

### Step 1 — Load historical actions

In one of the matches, click Reusable actions to load that Kata's historical actions.

![Selective Action Copy — View actions toggle expanded for a match](.gitbook/assets/selective-action-copy_view-actions-toggle-expanded-for-a-mat.png)

### Step 2 — Select the actions to import

Use the checkboxes to pick individual actions, or use Select All / Deselect All to act on the entire Kata.

![Selective Action Copy — checkboxes and Select All/Deselect All controls](.gitbook/assets/selective-action-copy_checkboxes-and-select-all-deselect-all.png)

### Step 3 — Combine selections from multiple Katas

Optionally repeat for other matches: selection persists across multiple Katas in the same session.

![Selective Action Copy — multi-Kata selection with total counter visible](.gitbook/assets/selective-action-copy_multi-kata-selection-with-total-counte.png)

### Step 4 — Import the selected actions

Click "Import N Actions" at the bottom of the modal.

![Selective Action Copy — Import N Actions button](.gitbook/assets/selective-action-copy_import-n-actions-button.png)

### Step 5 — Confirm and verify the import

The modal closes, a confirmation appears, and the current Kata's Actions table refreshes with the new records (Status = Open, no Due date).

![Selective Action Copy— modal closes and confirmation appears](.gitbook/assets/selective-action-copy—-modal-closes-and-confirmation-appears.png)

### Step 6 — Check the imported actions

Open the Kata where the Kata Similarity has been activated, in this example “Station 3 Scrap Rate Exceeding Threshold — OEE Loss on Line AI 1” and the current Kata's Actions table refreshes with the new records (Status = Open, no Due date).

![Selective Action Copy — current Kata Actions table refreshed with imported records](.gitbook/assets/selective-action-copy_current-kata-actions-table-refreshed-w.png)

## 3.6  Reading the result

Each match returned by Historical Lookup is scored and presented with the following information:
- Similarity score — A percentage (0-100) indicating how closely the closed Kata matches the open one. Scores above 70 indicate a strong thematic overlap; scores below 40 are weak matches shown for completeness.
- Why it matches — A concise AI-generated explanation of the shared elements between the two Katas (for example: same production area, same root-cause category, comparable KPI deviation).
- Key Differences — A brief summary of what distinguishes the historical case from the current one, helping you decide whether the historical resolution is directly applicable.
- Reusable actions — When the Reusable actions toggle is expanded, the full list of actions from the historical Kata is shown with their original title, description, and owner, ready for selective import into the current Kata.

## 3.7  Tips & known limits

By default Historical Lookup searches only inside the current Plant. The search perimeter is a customer-level configuration: when multi-plant scope is enabled for the Schneider GSC tenant, the source Plant is clearly labelled on every result so the user can judge cross-plant relevance.
Only Closed Katas are considered; in-progress Katas are excluded
Identical or near-identical Katas are not hidden — they appear with very high similarity so you can decide whether to import their actions
Imported actions always start fresh (Status = Open, Due date cleared): the new owner takes ownership of timing
Filters on Area, Line, Source, KPI are NOT hard filters — the AI uses them as semantic context, which means a relevant match from a different Line may still be proposed
