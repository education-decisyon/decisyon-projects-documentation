# 5  MEETINGSENSE

## 5.1  What it is

MeetingSense is the meeting recording and transcription capability embedded in DISS. It transforms the spoken dialogue of a SIM meeting into structured, digital data: a textual transcription, an executive summary, the issues raised, and a list of proposed actions ready to be added to the SIM action plan. The session is automatically contextualised with the metadata of the SIM Board it was launched from (Plant, SIM level, Production Area) so that every output is already linked to the right operational scope.

## 5.2  When to use it

During a daily SIM 2 meeting where a team discusses problems, root causes, and corrective actions and wants every outcome traceable in DISS without manual note-taking
Whenever the SIM Leader wants the conversation recorded in full so that nothing is lost between the discussion and the action plan
When the team needs both an attendance record and a structured set of actions ready to be assigned in one go at the end of the meeting

## 5.3  Prerequisites

The SIM Board on which the meeting is opened must be a SIM 2 Board (MeetingSense is enabled at this SIM level)
A working microphone must be available on the device used to start the meeting — without audio hardware the recording step displays an error
Attendance roles must be configured for the SIM 2 Board — the configuration is accessible at Plant Configuration → Attendance → SIM 2 Attendance Configuration
The user must have permission to start a meeting on the SIM Board in scope

## 5.4  How to use it

### Step 1 — Open the SIM Board and start the meeting

Navigate to the SIM Board where the meeting takes place (for example: Digitized Idea & SIM System → SIM Boards → SIM 2). On the board, the Plant, the Production Area and the Date are pre-filled. Click the Start Meeting button in the top-right corner to open the meeting initialisation dialog.

![SIM Board with Start Meeting button highlighted in the top-right corner](.gitbook/assets/sim-board-with-start-meeting-button-highlighted-in-the-top-r.png)

### Step 2 — Initialise attendance and Leader

The system automatically replicates the meeting context (Plant, SIM level, Production Area) so it does not need to be entered again. In the initialisation dialog:
Define the status of each participant: On time, Late, Absent, or Not Required
Assign the SIM Leader — by default the current user, changeable via dropdown
Confirm the settings and click Start Meeting to proceed
Meeting initialisation dialog with attendance statuses and SIM Leader selector

### Step 3 — Select the audio input and start recording

Choose the desired microphone from the list of available audio inputs and confirm. If no microphone is detected, an error message is displayed and the recording cannot be started.

![Audio input device selection popup with a microphone confirmed](.gitbook/assets/audio-input-device-selection-popup-with-a-microphone-confirm.png)

### Step 4 — Conduct the meeting

Speak clearly throughout the meeting and articulate the elements that will be needed to create the actions afterwards:
A short description of the problem discussed
The relevant Category (e.g. Safety, Quality, Delivery, Maintenance, Production, Engineering)
The name of the person assigned to the action
The target completion date
A pre-defined timeout protects against meetings left open by mistake: a notification dialog appears two minutes before the timeout to give the user a chance to extend or stop the session manually.

![Recording widget in active state during the meeting, with session duration and audio status indicator](.gitbook/assets/recording-widget-in-active-state-during-the-meeting,-with-se.png)

### Step 5 — Stop the recording and let the transcription process

Click the Stop control when the meeting is over. The system starts processing the audio in the background. While the transcription is being generated, you can move on to other activities — the team does not need to wait on the meeting page. A notification confirms when the transcript and the AI analysis are ready.

![Recording stopped, processing indicator and confirmation that transcription is queued](.gitbook/assets/recording-stopped,-processing-indicator-and-confirmation-tha.png)

### Step 6 — Open the meeting from the archive

Use the sidebar to navigate to Meeting → Overview Meeting. The Overview Meeting page lists every recorded session in chronological order, showing for each meeting: title, SIM level, date, and SIM Leader.

![Overview Meeting archive with the list of recorded sessions](.gitbook/assets/overview-meeting-archive-with-the-list-of-recorded-sessions.png)

Click on a meeting to open its detail view, where the AI-generated outputs are displayed together with the meeting metadata.

![Meeting detail view: Summary, Identified Issues, AI-suggested actions, duration, attendance record](.gitbook/assets/meeting-detail-view:-summary,-identified-issues,-ai-suggeste.png)

### Step 7 — Review and edit the transcript

To inspect the raw conversation, click Show Transcription: the verbatim text is displayed and remains fully editable. Correct any misinterpretation made by the speech-to-text engine or add details that were said but not picked up. When the transcript is updated, click Generate meeting notes to refresh the AI summary based on the new content.

![Transcript pane with Show Transcription opened and Generate meeting notes button](.gitbook/assets/transcript-pane-with-show-transcription-opened-and-generate-.png)

## 5.5  Reading the result

When the meeting detail view opens, MeetingSense exposes the following structured blocks for the SIM team:
- Summary — A narrative overview of the meeting discussion generated by the AI, covering the main topics addressed during the session.
- Identified Issues — A structured list of the problems and anomalies surfaced during the meeting, as extracted by the AI from the recorded conversation.
- AI-Suggested Actions — Action proposals generated automatically from the dialogue. Each suggestion includes an inferred description, category, owner, and due date — ready for review and direct assignment in DISS.
- Attendance Record — The attendance list compiled at the start of the meeting, with the status set for each participant: On time, Late, Absent, or Not Required.
- Duration — The total duration of the recorded meeting session.

## 5.6  Tips & known limits

Speak clearly and avoid overlapping voices: AI extraction quality scales with audio clarity. Articulate problem descriptions, owners and dates explicitly to maximise the accuracy of the AI-suggested actions.
Mention names and dates with precision — "John, by Friday" produces a stronger AI suggestion than implicit references such as "him, by end of week"
Category and Owner are mandatory for action creation: an action proposed without those values must be completed in the validation table before it can be saved
The transcript and the resulting actions are stored within the DISS tenant of your plant and are subject to the standard data-access rules
MeetingSense is a recording assistant: the SIM Leader is always in control — actions become part of the SIM plan only after explicit validation, and the transcript can be edited and re-summarised before any action is created
A pre-defined timeout protects against forgotten recordings: a 2-minute warning is shown before the session is closed automatically
