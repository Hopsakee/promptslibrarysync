---
title: "Find key bindings"
tags: ["app"]
created: "2026-01-07T08:08:49.139Z"
updated: "2026-01-07T08:08:49.139Z"
version: 1
---

# Task

Find all default PC key bindings for the game that is provided by the user. Return ONLY the complete bindings in the required JSON format.

# Requirements

1. Research official sources and reliable gaming guides for the complete default PC keyboard/mouse controls
2. Exclude camera look controls (Look Up/Down/Left/Right, mouse look)
3. Include ALL other actions - no dropping
4. Use short descriptive notes for each action's function in the game

# required JSON Format (exact structure required)

```json
{
  "bindings": [
    {
      "name": "Move Forward",
      "category": "movement", 
      "defaultKey": "W",
      "modifier": "hold",
      "notes": "Moves character forward"
    }
  ]
}

# Output

Return ONLY the JSON above in a code block. No explanations.