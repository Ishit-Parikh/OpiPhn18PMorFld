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
| Section 3: Snow Surfer | 31–59 | Done (completed 7th July) |

---

## Daily Logs

### 18th June 2026 (Thursday)

**Objective 1**
- **Start Time:** 3:30 PM
- **End Time:** 4:38 PM
- **Done:** Created a basic program demonstrating variables, data types, methods, classes, and objects.

---

### 19th June 2026 (Friday)

Had to complete yesterday's pending objectives along with new ones to stay on track.

**Objective 2 (Yesterday's objective)**
- **Start Time:** 11:21 AM
- **End Time:** 1:30 PM
- **Done:** Started the Unity 2D course. Learned the basic Unity interface — how to set scripts, choose the editor, and set/transform sprites from the Inspector Panel and via scripts.

**Objective 3 — Making a Simple Dodge Game**
- **Start Time:** 3:40 PM
- **End Time:** 5:55 PM
- **Done:** Understood colliders and triggers. Took a tea break and ran errands. Still needed more study to start and complete DodgeCube.

**Objective 3 (Continued)**
- **Start Time:** 7:30 PM
- **End Time:** 8:47 PM
- **Done:** Created a simple dodge game. Made the cube move left and right, and the ball fall from the sky. When the ball goes out of range, its position resets to Y = 0 with a random X value.

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

Extracted usable concepts for DodgeCube improvements. Took notes on what could be improved and what new mechanics could be borrowed.

---

### 26th June 2026 (Thursday)

**Lane B — Build DodgeCube v2 (Main Work)**

Transformed DodgeCube from prototype to a proper mini game.

**Objective 1 — Refactor Existing Code**
- Fixed `Player.cs` — removed dead code, replaced hardcoded speed values, cleaned up method naming
- Renamed falling object script from `StuffThatNeedsToBeDodged` → `Obstacle.cs`
- Fixed broken `Random.Range(5f, 4f)` → correct `Random.Range(-4f, 4f)`

**Objective 2 — Add Tags**
- Created tag: `Obstacle`
- Implemented tag-based collision detection
- Player hit by obstacle → game over (tag: `Player`)
- Ground collision → score +1 (tag: `Ground`)

**Objective 3 — Add Score**
- Every obstacle successfully dodged (hits ground) increments score by 1
- Score tracked in `GameControll.cs`

**Objective 4 — Add UI**
- TextMeshPro score display: "Score: 0"
- Positioned top-left
- Updated via `updateScore()` method

---

### 27th June 2026 (Saturday)

**Session Stretch 1**
- **Start Time:** 3:40 PM
- **End Time:** 10:30 PM
- **Done:**
  - Renamed scripts and updated GitHub to reflect the changes
  - Added game states to support launching MainMenu and GameOver screens
  - Implemented MainMenu and GameOver logic with multiple breaks in between
  - Undid the entire progress at the end — the multi-scene logic required significant recalibration and cleanup was too messy. Will restart fresh tomorrow from where I left off.

---

### 28th June 2026 (Sunday)

**Session Start**
- **Start Time:** 6:15 PM
- **End Time:** 9:10 PM
- **Done:**
  - Added dynamic bounds to player movement limits based on camera view (completed by 6:40 PM)
  - Built Main Menu UI using Canvas (no new scene). UI includes a title logo and a game start button.

---

### 29th June 2026 (Monday)

**Session Start**
- **Start Time:** 2:15 PM
- **End Time:** 6:10 PM
- **Done:**
  - **Objective 4 — Create GameManager Properly**
    - Created `GameManager.cs` to centralize score, game state, UI panels, spawning, and start/game over logic
    - Key variables: `isGameActive`, `isGameOver`, `score`, `finalScore`
    - `GameStart()` — sets game active, shows score panel
    - `SpawnPlayer()` — instantiates player at fixed position
    - Dynamic player bounds using `Camera.main.ViewportToWorldPoint()` with padding
    - `Update()` flow: if game active → spawn player + obstacles; if game over → show game over panel
    - Score panel hidden initially, shown on game start
  - **Objective 5 — Start Button Logic**
    - On Start click: `GameStart()` sets `isGameActive = true`, shows score panel
    - `Update()` loop then spawns player and obstacles automatically
    - Game only runs after clicking Start
  - **Objective 6 — Game Over Screen**
    - GameOverPanel with GAME OVER text, final score display, and Restart button
    - Panel hidden initially, shown via `GameOverPanel()` method on death
    - Displays final score from `finalScore` variable
  - **Objective 7 — Stop Gameplay on Death**
    - `PlayerController.Update()` checks `isGameActive` before processing input
    - `Obstacle` on Player trigger: sets `isGameActive = false`, `isGameOver = true`
    - `GameManager.Update()` stops spawning when game is inactive
    - Player movement uses `Mathf.Clamp` with dynamic bounds from GameManager
  - **Objective 8 — Restart Button**
    - Soft restart via `RestartGame()` — resets score/finalScore to 0, calls `GameStart()`
    - GameOverPanel hidden, score panel shown, player re-spawns
  - **Objective 9 — Final GitHub Push**
    - Renamed `BoppyMovement.cs` → `PlayerController.cs`, `GameControll.cs` → `GameManager.cs`
    - Pushed all changes to remote repository

---

### 30th June – 2nd July 2026 (Break)

No progress — mouse developed a severe double-clicking issue. Unable to work effectively in Unity.

---

### 3rd July 2026 (Friday)

New mouse arrived. Back on track.

**Session 1 — Course Progress**
- **Start Time:** 3:00 PM
- **End Time:** 5:00 PM
- **Done:** Watched Section 3: Snow Surfer, **Lectures 31–40**
  - **Lecture 31–32:** Section intro and game design breakdown — rolling ball, slopes, obstacles, powerups
  - **Lecture 33–34:** Sprite Shapes for 2D terrain and Edge Colliders for physics collision
  - **Lecture 35:** Cinemachine Follow Camera with damping and look-ahead
  - **Lecture 36–37:** Setting up the ball character with Rigidbody2D, Surface Effector 2D for slope sliding
  - **Lecture 38:** Unity's modern Input System — Input Actions, key bindings, Vector2 input
  - **Lecture 39:** Rotating the player using `AddTorque()`
  - **Lecture 40:** Finish Line & Crash Detector trigger zones with `OnTriggerEnter2D()`

**Session 2 — Hands-On Implementation**
- **Start Time:** 6:30 PM
- **End Time:** 8:30 PM
- **Done:** Implemented Snow Surfer concepts in a practice Unity project
  - Set up Input System bindings with `InputSystem.actions.FindAction("Move")`
  - Applied `AddTorque` to Rigidbody2D for ball rotation based on input
  - Created `FinishLine.cs` — detects player layer trigger, logs win
  - Created `CrashDetector.cs` — detects floor layer trigger, logs crash
  - Used LayerMask for clean collision detection instead of tags

---

### 4th July 2026 (Saturday)

**C# MasterClass — Section 3: Loops**
- **Done:**
  - `for` loops, `foreach` loops, nested loops
  - Arrays and jagged 2D arrays
  - **RocketLanding.cs** — countdown timer with `for` loop, ASCII animation with `Thread.Sleep`
  - **CodeExe7.cs** — `foreach` loop iterating over an int array
  - **CodeExe8.cs** — nested `for` loops summing rows of a jagged 2D array

---

### 5th July 2026 (Sunday)

**C# MasterClass — Section 4: Functions & Methods**
- **Done:**
  - Method declaration, parameters, return types
  - **CodeExe9.cs** — `CalculateAverage()` method taking a `double[]` parameter and returning the average; `PrintAverage()` calling it and outputting the result

---

### 6th July 2026 (Monday)

**Unity 2D Course — Lectures 41–50 (Snow Surfer continued)**
- **Done:**
  - **Lecture 41–42:** `SceneManager.LoadScene()`, `Invoke()` for delayed scene restart
  - **Lecture 43–44:** Particle Systems — configuring emission, shape, color, burst; triggering `Play()` / `Stop()` from code
  - **Lecture 45:** Game feel tuning — physics values, background sprites
  - **Lecture 46:** `FindFirstObjectByType<T>()` for dynamic Surface Effector boost
  - **Lecture 47:** `OnCollisionExit2D()` — snow particles play on ground contact, stop on exit
  - **Lecture 48:** Public access modifier — `canControllPlayer` bool to disable input on crash
  - **Lecture 49:** Flip counting with `Mathf.DeltaAngle()` and `Transform.eulerAngles`
  - **Lecture 50:** Function parameters — `updateScore(int addScore)` for reusable scoring

**Implemented alongside the instructor:**
  - `SnowParicleScript.cs` — `OnCollisionEnter2D` / `OnCollisionExit2D` with LayerMask for particle control
  - `ScoreManager.cs` — `updateScore(int addScore)` method with parameter
  - `PlayerController.cs` — `flipCounts()` with `Mathf.DeltaAngle`, `boostPlayer()` with `SurfaceEffector2D.speed`, `canControllPlayer` state
  - Crash/win scene transitions with `SceneManager.LoadScene()` and `Invoke()`

---