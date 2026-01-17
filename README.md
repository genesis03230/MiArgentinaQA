# Mi Argentina – QA Manual Testing

## Project Overview
Mi Argentina is a first-person escape room puzzle game developed in Unity.

- Engine: Unity 2021.3.12f1
- Platform: PC
- Game Type: Puzzle / Escape Room
- Status: Playable

## Core Objective
The player must collect the 23 provinces of Argentina and place them correctly on the map to unlock the exit door and complete the game.

## QA Scope
The QA activities for this project focus on:
- Gameplay progression validation
- Object interaction and lifecycle
- Physics and boundary handling
- Prevention of soft locks and unrecoverable states
- User experience and error tolerance

## Known Risk Areas
- Raycast-based object interaction
- Dropping and recovering collectible items
- Objects leaving the playable area
- Missing respawn or recovery mechanisms

## Visual QA Preview

The following preview demonstrates a critical issue identified during manual testing.  
In this scenario, a collectible province can be dropped outside the playable area, becoming unrecoverable and preventing game completion without restarting.

![Province lost outside playable area](Evidence/bug_province_lost.gif)

> Full reproduction steps, severity, and complete video evidence are documented in `Bug-Reports.md`.

## Test Artifacts
- 📄 [Manual Test Cases](Test-Cases.md)
- 🐞 [Bug Reports with Evidence](Bug-Reports.md)
