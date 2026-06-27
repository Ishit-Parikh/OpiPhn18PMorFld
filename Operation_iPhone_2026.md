# Operation iPhone 2026

## Why

Become employable as a Game Developer and earn enough to purchase the latest iPhone using money earned through my own work.

## Timeline

- **Start Date:** 18 June 2026
- **Target Date:** 30 September 2026

## Projects

### DodgeCube

A simple 2D dodge game built with Unity while learning the engine.

- **Repository:** [Ishit-Parikh/DodgeCube](https://github.com/Ishit-Parikh/DodgeCube)
- **Unity Version:** 6000.3.18f1

## Course: Complete C# Unity 2D Game Development

- **Platform:** Udemy
- **Course URL:** https://www.udemy.com/share/101Wjs/

Coverage:

| Section | Lectures | Status |
|---------|----------|--------|
| Section 1: Introduction & Setup | 1–6 | Done |
| Section 2: Delivery Dash | 7–30 | Done (completed 25th June) |

---

## Daily Logs

### 18th June 2026 (Thursday)

**Objective 1**
- **Start Time:** 3:30 PM
- **End Time:** 4:38 PM
- **Done:** Created a basic program that demonstrates the use of variables, data types, methods, classes, and objects.

---

### 19th June 2026 (Friday)

Had to complete yesterday's incomplete objectives as well as new ones today to be on track.

**Objective 2 (Yesterday's objective)**
- **Start Time:** 11:21 AM
- **End Time:** 1:30 PM
- **Done:** Started the Unity 2D course. Learnt the basic interface for Unity including how to set scripts, editor of choice, set and transform sprites from the Inspector Panel & via scripts.

**Objective 3 — Making a Simple Dodge Game**
- **Start Time:** 3:40 PM
- **End Time:** 5:55 PM
- **Done:** Understood how to set colliders and Triggers. Took a tea break & ran some errands. Still needed to learn more to start and complete DodgeCube.

**Objective 3 (Continued)**
- **Start Time:** 7:30 PM
- **End Time:** 8:47 PM
- **Done:** Created a simple game where all you have to do is dodge the falling ball. Made the Square Sprite (Cube) move left and right & made the ball fall from the sky. If ball goes out of range, its position is reset with Y being 0 and a random X value.

---

### 25th June 2026 (Wednesday)

**Lane A — Course Progress (Max 90 mins)**

Continued Section 2: Delivery Dash from **Lecture 19 → Lecture 30**.

Concepts covered:
- Importing assets
- Tags
- Bools
- Prefabs
- Destroy
- GetComponent
- Boosts & bumps
- UI text

Extracted usable concepts for DodgeCube improvements. Took notes on what could improve the game and what new mechanics to borrow.

---

### 26th June 2026 (Thursday)

**Lane B — Build DodgeCube v2 (Main Work)**

Transformed DodgeCube from prototype to actual mini game.

**Objective 1 — Refactor Existing Code**
- Fixed `Player.cs` — removed dead code, replaced hardcoded speed values, cleaned method naming
- Renamed falling object script from `StuffThatNeedsToBeDodged` → `Obstacle.cs`
- Fixed broken `Random.Range(5f, 4f)` → correct `Random.Range(-4f, 4f)`

**Objective 2 — Add Tags**
- Created tag: `Obstacle`
- Implemented tag-based collision detection
- Player hit by obstacle → game over (tag: `Player`)
- Ground collision → score +1 (tag: `Ground`)

**Objective 3 — Add Score**
- Every obstacle successfully dodged (hits ground) increments score by 1
- Score tracking in `GameControll.cs`

**Objective 4 — Add UI**
- TextMeshPro score display: "Score: 0"
- Positioned top-left
- Updated via `updateScore()` method
