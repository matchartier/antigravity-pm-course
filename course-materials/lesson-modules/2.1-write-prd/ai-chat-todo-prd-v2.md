# PRD: TaskFlow "Async Voice" (Draft v2)

# Problem Alignment

## Problem & Opportunity

**Problem:** Distributed teams struggle with the loss of nuance in text-only task assignments. Typing out complex instructions is tedious, so tasks are often vague ("Fix this"), leading to back-and-forth and delays.

- **Why:** Remote work relies on Async Communication. We need to make Async as rich as Sync (meetings) without the scheduling cost.
- **Insight:** Users chose "Natural Interface" as a key need; they want the ease of talking without the pressure of a meeting.
- **Urgency:** High. "Zoom fatigue" is real; shifting work to async voice reduces meeting load.

## High Level Approach

**Solution:** "TaskFlow Voice": A voice-first task creator that emphasizes _context_. Users speak tasks naturally. The AI doesn't just transcribe; it interprets intent and attaches the voice clip for emotional context/nuance.

**Alternatives:** Video messages (Loom style). Rejected for now as too heavy/bandwidth intensive for simple to-do items.

### Narrative

_Scenario:_ A Product Manager finds a bug. Describing it in text takes 5 minutes of typing steps. With TaskFlow Voice, they record: "Hey engineering, when I click this button, it feels laggy. Can we check the latency? assigning to Dave." Dave gets the task, reads the AI summary, and listens to the clip to hear the tone/urgency.

## Goals

1.  **Communication Clarity:** Reduce "comments per task" on voice-created tasks (indicating clearer initial instruction).
2.  **Engagement:** 15% of tasks created contain voice context.
3.  **Differentiation:** Establish TaskFlow as the "Human" remote tool.

## Non-goals

1.  **Chatbot Chit-chat:** The AI is a tool, not a friend. No personality mode.
2.  **Complex project creation:** Usage is limited to Tasks and Subtasks, not creating full Project spaces.

# Solution Alignment

## Key Features

1.  **Smart Transcription:** Converts speech to structured task data (Who, What, When).
2.  **Voice Context Player:** Embedded player in the task card for the original audio.
3.  **"Edit with Voice":** Use voice commands to update existing tasks ("Move this to Done").

### Key Flows

1.  **Capture:** User taps Mic -> Speaks -> AI Drafts Task -> User Confirms.
2.  **Clarify:** Assignee listens to audio -> Responds with text or voice comment.

### Key Logic

1.  **Complexity Management:** To avoid cognitive load, the voice interface is hidden behind a single "Mic" icon. It does not clutter the main UI.
2.  **Permissions:** Browser/Phone microphone permissions must be handled gracefully.

# Development and Launch Planning

| Milestone       | Target Date | Description                           |
| --------------- | ----------- | ------------------------------------- |
| Kickoff         | Week 1      |                                       |
| Design Complete | Week 2      | Focus on "Waveform" visualization     |
| Dev Complete    | Week 6      |                                       |
| Beta            | Week 7      | release to "Power User" segment first |
| Launch          | Week 9      |                                       |

## Operational Checklist

- [ ] Legal: Update Terms of Service regarding audio data storage / processing.
- [ ] Infrastructure: Ensure storage bucket capacity for audio files.
