---
name: Bug Report
about: Report an issue or unexpected behavior in the EcoSnap Mobile App.
title: "[BUG] Short, descriptive summary of the issue"
labels: ["bug", "triage"]
assignees:

---

## 1. Context & Environment

**(REQUIRED) Describe the environment where the bug occurred. Be precise. Adhering to the Apex Standard means detailed context is mandatory for fast resolution.**

*   **Application Version:** (e.g., v1.2.0 or latest commit hash)
*   **Platform:** (iOS / Android / Web Simulator)
*   **Device Model:** (e.g., iPhone 15 Pro, Samsung Galaxy S24)
*   **OS Version:** (e.g., iOS 18.1, Android 15)
*   **React Native/Expo Version:** (If applicable, check `package.json`)

## 2. Description of the Bug

A clear, concise description of what the bug is and what you expected to happen.

**Expected Behavior:**

*What should have happened?*

**Actual Behavior:**

*What actually happened?*

## 3. Reproduction Steps

**(CRITICAL) Provide the exact, repeatable steps necessary to trigger this bug. Use numbered lists. If this cannot be reproduced, the ticket may be closed by the triage agent.**

1.  Launch the application.
2.  Navigate to the [Screen Name] screen.
3.  Tap the [Button Name] button.
4.  Capture an image of [Specific Object].
5.  Observe the output classification.

## 4. Evidence (Screenshots / Logs)

Attach any relevant screenshots, screen recordings, or crash logs here. For logs, please use a service like Pastebin or Gist and link them below.

*   [Link to Screenshot 1]
*   [Link to Log File]

## 5. Architectural Analysis (Optional but Encouraged)

If you suspect which component is failing (e.g., TypeScript type mismatch in the prediction service, image tensor processing on the client), describe it here. This leverages the Modular Monolith understanding of the project structure.

*Example: It seems the image preprocessing utility (`src/utils/imageTransform.ts`) is failing to correctly resize the input tensor before sending it to the ML model endpoint.*

## 6. Priority Assessment

*   **[ ] Blocker:** Prevents core functionality (e.g., image capture fails entirely).
*   **[ ] Critical:** Major feature degradation (e.g., incorrect classification for 50% of common items).
*   **[ ] Major:** Significant UX issue or minor feature failure.
*   **[ ] Minor:** Cosmetic issue or edge-case failure.
