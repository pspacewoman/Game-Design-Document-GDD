## Game Design Document Bundle
What the game is, how it plays, its systems, features, and design decisions. Concept clarity and communication with the team.

# 🎮 Game Design Document (GDD)

**Projects:**
**Version:** 1.0 
**Author:** Priyanshi Singh  

a. Emergency Quest (VR) — Master Thesis prototype
b. DeadZone — FPS 3D Shooter
c. 3D Solar System — Interactive Simulation

---

Table of contents-

1. Emergency Quest (VR)
2. DeadZone — FPS
3. 3D Solar System
4. Common repo & workflow templates
5. Playtesting, metrics & accessibility
6. Export to GitHub quick-start checklist

---

## Emergency Quest (VR)
Overview / Elevator Pitch:

Emergency Quest is an immersive VR training game for Meta Quest devices where players respond to road-accident scenarios to practice first-aid, triage, and decision-making under pressure. The game combines realistic environments, NPC animations, and guided feedback for learning outcomes.

## Target audience & learning goals

- Primary: learners and trainees (medical volunteers, high school/uni safety programs).
- Secondary: general VR players interested in realistic simulations.
- Learning goals: recognize accident types, triage priority, apply basic first-aid (CPR, bleeding control), and practice communication & empathy.

## Core gameplay loop
- Receive dispatch & move to accident scene.
- Assess victims & environmental hazards.
- Apply first-aid actions (bandaging, CPR, stop bleeding, repositioning).
- Get scored on correctness, time, and safety.
- Receive instructor feedback, repeat with adjusted difficulty.

## Key features (MVP / v1 / stretch)
- MVP: 3 accident scenarios (car crash, bike collision, pedestrian fall), interactive tools (bandage, tourniquet, CPR), scoring & instructor HUD.
- v1: Branching scenarios, NPC dialogue trees, environmental hazards (fire, broken glass), replayable scenarios with analytics.
- Stretch: Multiplayer instructor mode, learning management system (LMS) export, adaptive difficulty via analytics.

## Controls & interaction
- XR Interaction Toolkit interactable objects (grab, place, use).
- Teleport + smooth locomotion toggle for comfort.
- Contextual radial menu for tools and instructions.
- Haptics for success/failure feedback.

## Level design & flow
- Intro tutorial (tool use, movement).
- Scenario 1: simple single-victim — focus on assessment.
- Scenario 2: multi-victim — prioritization & triage.
- Scenario 3: environmental hazard — scene safety, extrication.

## Story & Characters
- Non-heavy story; scenario-based vignettes with short hero NPCs and a dispatcher voice guiding players.

## Art & Audio
- Semi-realistic low-poly assets mixed with high-fidelity audio cues (breathing, groans, ambient traffic).
- UI: diegetic hints + non-diegetic HUD for scores and instructions.

## Technical spec & Unity notes
- Engine: Unity LTS (recommended 2022.3+ or latest LTS at start). Use URP for performance on Quest.
- Target: Meta Quest 3 / Quest 2 (build configs included).
- Packages: XR Interaction Toolkit, Oculus Integration / Meta XR SDK, Cinemachine, TextMeshPro, DOTS (optional), Unity Analytics or a lightweight custom telemetry.
- Physics: Rigidbody-based interactions, kinematic ragdoll transitions for NPCs.

## UX & Usability (important for training)
- Comfort options: teleport/smooth locomotion, vignetting, adjustable height.
- Tutorials with guided hands-on practice.
- Clear feedback and post-scenario debrief screens.

## Playtesting & evaluation plan
- Iterative usability tests using task completion metrics and surveys.
- Logging: time-to-first-action, errors, incorrect procedures, tool selection path.

## Accessibility
Subtitles and large text options, color-blind-friendly palettes, options for left/right handedness.

---
