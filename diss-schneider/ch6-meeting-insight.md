# 6  MEETING INSIGHT

## 6.1  What it is

![Meeting Insight is an AI agent that works on top of the meetings already captured by MeetingSense. While MeetingSense focuses on a single recording, Meeting Insight analyses multiple meeting transcripts simultaneously to surface patterns, recurring issues, and aggregated action items across the whole archive. It transforms a stream of individual SIM minutes into operational intelligence at the plant or area level.](.gitbook/assets/meeting-insight-is-an-ai-agent-that-works-on-top-of-the-meet.png)

## 6.2  When to use it

To answer "What problems keep coming back?" — Meeting Insight identifies recurring themes across SIM meetings over a chosen period
To produce a consolidated list of action items from many meetings (for example, all SIM 1 meetings in the past month) without opening them one by one
To extract trends and patterns across different production dates and production areas, supporting management reviews and continuous-improvement steering
To investigate a topic across the meeting archive using natural-language questions in any supported language

## 6.3  Prerequisites

At least one meeting transcription produced by MeetingSense must exist in the DISS environment
The user must have access to the Overview Meeting archive
The user must have read access to the meetings included in the analysis

## 6.4  How to use it

### Step 1 — Navigate to the Overview Meeting archive

Navigate to the Overview Meeting archive in DISS.

![Meeting Insight — Overview Meeting archive page](.gitbook/assets/meeting-insight_overview-meeting-archive-page.png)

### Step 2 — Filter the meeting archive

Use date or organisational level filters to isolate the meetings relevant to your analysis scope.

![Meeting Insight — date and level filters on the archive](.gitbook/assets/meeting-insight_date-and-level-filters-on-the-archive.png)

### Step 3 — Select the meetings to analyse

Select multiple meetings using the checkboxes on the left of each row to define the analysis dataset.

![Meeting Insight — meetings selected via checkboxes](.gitbook/assets/meeting-insight_meetings-selected-via-checkboxes.png)

### Step 4 — Launch Meeting Insight

Click "Summarize Notes" to launch the Insight Agent on the selected meetings.

![Meeting Insight — Summarize Notes button](.gitbook/assets/meeting-insight_summarize-notes-button.png)

The agent opens a dialog window where you can interact with the combined dataset of all selected transcripts.

![Meeting Insight — dialog window opened with combined dataset](.gitbook/assets/meeting-insight_dialog-window-opened-with-combined-dataset.png)

### Step 5 — Manage the active selection

Use the side panel to view or deselect specific meetings without closing the dialog, keeping full control over the analysis scope.

![Meeting Insight — managing the active selection from the dialog](.gitbook/assets/meeting-insight_managing-the-active-selection-from-the-dialo.png)

### Step 6 — Extract the list of action items

Click "Extract list of action items" to aggregate all action items across the selected sessions in a single list.

![Meeting Insight — action items list aggregated across meetings](.gitbook/assets/meeting-insight_action-items-list-aggregated-across-meetings.png)

### Step 7 — Ask natural-language questions

Ask personalised natural-language questions in the input field to locate specific operational details (root causes, recurring barriers, owners, etc.) across the transcripts.

![Meeting Insight — natural-language query on the selected meetings](.gitbook/assets/meeting-insight_natural-language-query-on-the-selected-meeti.png)

### Step 8 — Export and bookmark results

Optionally bookmark frequently used queries for faster reuse, and copy the generated summaries or action lists to external documents for reporting.

![Meeting Insight — bookmarking a query and exporting the results](.gitbook/assets/meeting-insight_bookmarking-a-query-and-exporting-the-result.png)

## 6.5  Reading the result

![Meeting Insight presents its output directly in the dialog window opened by Summarize Notes. The type of result varies depending on the interaction performed:](.gitbook/assets/meeting-insight-presents-its-output-directly-in-the-dialog-w.png)

- Action items list — Clicking Extract list of action items produces a consolidated, deduplicated list of all action items surfaced across the selected meeting sessions, showing description, inferred owner, and source meeting.
- Natural-language response — Submitting a free-text query returns a synthesised AI answer drawing on the full transcribed content of the selected meetings. The response indicates the meeting and session where the relevant content was found.
- Bookmarked queries — Frequently used queries can be saved and reused from the side panel, accelerating recurring analyses such as weekly trend checks or management reviews.
- The results are advisory. The meeting leader remains responsible for converting recurring patterns into concrete countermeasures via the Actions feature.

## 6.6  Tips & known limits

Quality of insights scales with the quality of the underlying MeetingSense minutes: encourage clean recordings and explicit naming of owners and dates during meetings
Use filters before launching the agent — analysing a focused dataset (for example one SIM level and one month) yields sharper insights than scanning the entire archive
Real-time AI participation during the SIM meeting itself is not part of this release: Meeting Insight today operates on already-recorded minutes. Live participation is tracked as a future enhancement.
Insights are advisory: the leader is responsible for translating recurring patterns into concrete countermeasures via Actions or Katas
