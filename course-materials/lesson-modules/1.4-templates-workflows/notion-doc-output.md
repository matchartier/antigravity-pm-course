# Onboarding Research Findings - May 2024

**Author:** Sarah Chen, Senior PM
**Last Updated:** May 10, 2024

## Overview

Research findings from 12 user interviews and analytics deep-dive investigating the 40% drop-off at the "Invite Team" onboarding step. This doc outlines the "Solo User" churn pattern and recommends UI changes to improve collaboration adoption.

## Background / Context

We observed that 40% of new workspaces never invite a second user. We hypothesized that these users churn at higher rates. This research validates that hypothesis and explores _why_ users skip the invite step.

## Key Findings

### 1. The "Solo User" Churn Pattern

Solo users are 3x more likely to churn than teams.

- **Churn Rate:** 68% (Solo) vs 22% (Teams)
- **Usage:** Solo users avg 4 min sessions vs 18 min for teams
- **Impact:** 272 failed workspaces/month (~$4k MRR loss)

### 2. Value Prop Disconnect

Users fundamentally misunderstand the product when onboarding alone.

- 34% believe TaskFlow is for "personal task management"
- Quote: "I wanted to try it first before inviting my team" (leading to 4-min session → churn)

### 3. Frictionless Skipping

The current UI encourages skipping the invite.

- 73% click "Skip for now"
- Only 12% ever return to invite a team member later

## Implications

- **Revenue:** We are losing ~$48k/year in potential ARR due to poor onboarding conversion.
- **Product Positioning:** Our "low friction" onboarding is actually hurting us by allowing users to experience the "wrong" version of the product (solo mode).

## Recommendations / Next Steps

### 1. Redesign Team Invite Step (High Impact)

Make team invitation central to the flow.

- **Owner:** Jamie (Design)
- **Target:** May 18

### 2. Implement Follow-up Email (Low Effort)

Send 24hr automated nudge to solo users.

- **Owner:** Alex (Eng)
- **Target:** May 20

### Success Metrics

- Reduce solo workspace creation from 40% to 25% in 60 days.

## References

- [Full Interview Transcripts](link)
- [Analytics Dashboard](link)
