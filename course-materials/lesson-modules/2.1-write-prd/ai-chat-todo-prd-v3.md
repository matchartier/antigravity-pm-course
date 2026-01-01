# PRD: TaskFlow AI Assistant - The Cognitive Unburdening (Draft v3)

# Problem Alignment

## Problem & Opportunity

**Problem:** Managing a project management tool is work in itself. For our target users (SMBs, 5-20 ppl), "Complexity Overwhelm" is the enemy. They avoid entering data because the UI feels like a cockpit.

- **Why:** If the tool feels like work, they churn.
- **Strategy:** Leverage "Natural Interface" (AI Voice) to bypass UI complexity entirely.
- **Risk:** We must avoid the "Clippy" effect where the assistant adds _more_ distraction.

## High Level Approach

**Solution:** An invisible interface. A background AI agent that listens to commands and executes them, removing the need to navigate the UI. It's not just "Voice to Text," it's "Voice to Action."

**Alternatives:** Command Palette (cmd+k). Good for power users, but voice is better for accessibility and multitasking.

### Narrative

_Scenario:_ A user is driving to a client site. They panic: "I forgot to email the proposal!" They tap one button on their phone: "Add a high priority task to the Sales project: Email proposal to Acme by 5pm today." The AI handles the categorization, tagging, and priority setting invisibly.

## Goals

1.  **Reduction in Clicks:** Reduce average clicks-to-create-task from 7 to 2.
2.  **Mobile Usage:** Increase mobile app session frequency by 25%.
3.  **Sentiment:** User feedback cites "It feels like magic" or "It's so easy."

## Non-goals

1.  **Visual Avatar:** No dancing robot icons. The interface is text/audio only.
2.  **Social Features:** No sharing voice clips publicly.

# Solution Alignment

## Key Features

1.  **Intelligent Parsing:** Deep understanding of relative dates ("Next Tuesday", "End of Sprint").
2.  **Context Awareness:** If I'm looking at Project A, and say "Add task," it assumes Project A.
3.  **Briefing Mode:** "Read me my tasks for today" (Output mechanism, not just input).

### Key Flows

1.  **Input:** Tap -> Speak -> Toast Notification "Task Added". (Optimized for speed, minimal review).
2.  **Correction:** "No, I meant next Tuesday." -> AI updates the draft.

### Key Logic

1.  **Confidence Threshold:** If confident > 90%, auto-create. If < 90%, ask for confirmation.
2.  **Error Handling:** If unheard, gentle "I didn't catch that," not technical error codes.

# Development and Launch Planning

| Milestone | Target Date | Description                                              |
| --------- | ----------- | -------------------------------------------------------- |
| Prototype | Week 2      | Wizard of Oz testing to validate specific voice commands |
| MVP Build | Week 5      | Restrict to "Create Task" intent only                    |
| Polish    | Week 7      | Focus on latency reduction (speed is key)                |
| Launch    | Week 8      |                                                          |

## Operational Checklist

- [ ] Analytics: specialized funnel for "Voice intent success rate".
- [ ] Marketing: positioning this as the "Antidote to Overwhelm."
