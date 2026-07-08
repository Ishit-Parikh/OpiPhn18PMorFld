# Operation iPhone 2026

> **Mission:** Become employable as a Game Developer and earn enough to purchase the latest iPhone using money earned through my own work.

## Timeline

| | Date |
|---|---|
| **Start** | 18 June 2026 |
| **Target** | 30 September 2026 |
| **Days Elapsed** | 21 |
| **Days Remaining** | 84 |

---

## Courses

### 1. Complete C# Masterclass

- **Repository:** [Ishit-Parikh/CSharp-Learning-Journey](https://github.com/Ishit-Parikh/CSharp-Learning-Journey)
- **Platform:** Udemy
- **Instructor:** Denis Panjuta
- **Duration:** 46h 12m · 484 lectures · 28 sections
- **URL:** https://www.udemy.com/share/1013Gg/

| Section | Status | Date Completed |
|---------|--------|----------------|
| 1 — Introduction, DataTypes & Variables | Done | Before 18th June |
| 2 — Making Decisions (if/else, switch) | Done | Before 4th July |
| 3 — Loops (for, foreach, while, arrays) | Done | 4th July |
| 4 — Functions and Methods | Done | 5th July |
| 5+ | Pending | — |

### 2. Complete C# Unity 2D Game Development (Updated To Unity 6)

- **Platform:** Udemy
- **Instructors:** GameDev.tv Team, Rick Davidson, Ahmed Nassef
- **Duration:** 17h 16m · 132 lectures · 6 sections
- **URL:** https://www.udemy.com/share/101Wjs/

| Section | Lectures | Status | Date Completed |
|---------|----------|--------|----------------|
| 1 — Introduction & Setup | 1–6 | Done | 19th June |
| 2 — Delivery Dash | 7–30 | Done | 25th June |
| 3 — Snow Surfer | 31–59 | Done | 7th July |
| 4 — Tilemania | 60–100 | Pending | — |
| 5 — Star Blaster | 101–130 | Pending | — |

---

## Projects

### BoppyDodge 

- **Repository:** [Ishit-Parikh/BoppyDodge](https://github.com/Ishit-Parikh/BoppyDodge)
- **Unity Version:** 6000.3.18f1
- **Type:** Self-made 2D dodge game (no tutorial)
- **Scripts:** `GameManager.cs`, `PlayerController.cs`, `Obstacle.cs`

### Snow Surfer Practice

- **Type:** Course-taught game + independent rebuild
- **Scripts:** `PlayerController.cs`, `ScoreManager.cs`, `CrashDetector.cs`, `FinishLine.cs`, `SnowParicleScript.cs`, `PowerUpManager.cs`, `PowerupSO.cs`

### DeliveryDash Practice

- **Type:** Course-taught practice
- **Scripts:** `Movement.cs`, `Delivery.cs`

### C# Masterclass Code

- **Type:** Console exercises following the C# Masterclass
- **Sections completed:** 1–4 (Intro, Decisions, Loops, Functions)

---

## Daily Logs

---

### 18th June 2026 (Thursday)

**Objective 1 — First C# Program**
- **Start Time:** 3:30 PM
- **End Time:** 4:38 PM

Wrote a foundational C# console program covering:
- **Variables** — declared `string`, `int`, `double`, `bool` variables and observed how each type behaves
- **Data types** — understood value types vs reference types, implicit and explicit conversion
- **Methods** — defined and called simple static methods to organize logic
- **Classes and Objects** — created a basic class with fields and methods, instantiated it in `Main()`

This was a warm-up to re-establish programming fundamentals before diving into Unity's C#.

---

### 19th June 2026 (Friday)

> Had to complete yesterday's pending objectives along with new ones to stay on track.

**Objective 2 — Unity 2D Course: Introduction & Setup**
- **Start Time:** 11:21 AM
- **End Time:** 1:30 PM

Worked through the initial setup of the Unity 2D course:
- **Lecture 4 — Start Using Unity:** Explored the Unity Editor interface — Scene view, Game view, Hierarchy, Inspector, Project panel, Toolbar. Created basic GameObjects (cube, sphere), manipulated transforms (position, rotation, scale).
- **Lecture 5 — Our First Code:** Wrote the first C# script in Unity. Learned about `MonoBehaviour`, the `Start()` method (runs once on enable) and `Update()` method (runs every frame). Used `Debug.Log("Hello World")` to verify the environment.
- Installed necessary modules (WebGL, Windows/Mac/Linux build support).

**Objective 3 — Making a Simple Dodge Game (Part 1)**
- **Start Time:** 3:40 PM
- **End Time:** 5:55 PM

Started building **DodgeCube** from scratch:
- **Colliders** — added Box Collider 2D to the player cube and falling obstacles
- **Triggers** — configured `isTrigger` on certain colliders for pass-through detection (pickups, zones)
- Took a break and ran errands. Still needed more study to complete the game.

**Objective 3 (Part 2)**
- **Start Time:** 7:30 PM
- **End Time:** 8:47 PM

Completed the first prototype of **DodgeCube**:
- Player cube moves left/right using keyboard input (`Input.GetKey`)
- Falling obstacles spawn at random X positions and drop downward via `Transform.Translate()`
- When obstacle goes off-screen (below camera), its position resets to Y = 0 with a new random X value
- Basic `Transform.Translate()` movement with `Time.deltaTime` for frame-rate independence

---

### 25th June 2026 (Wednesday)

**Lane A — Course Progress (Lectures 19–30)**

Worked through Section 2: **Delivery Dash** from **Lecture 19 → 30** (~2 hours of content).

| Lecture | Concept | What I Learned |
|---------|---------|----------------|
| 19 | Add Assets To Project | Importing sprites, audio, prefabs; sprite import settings (pixels per unit, filter mode, compression) |
| 20 | Car & Background | Applying sprites to GameObjects, tiling backgrounds with seamless textures |
| 21 | Create A Level | Level design in Scene view using sprites/props |
| 22 | Add Collision Blocks | Collision boundaries with Box Colliders, area collider approaches |
| 23 | Using Tags In Unity | Tag system for identifying GameObjects ("Obstacle", "Pickup", "FinishLine") |
| 24 | Introducing Bools | Boolean flags for tracking state (e.g., isBoosting) |
| 25 | Introducing Prefabs | Reusable GameObject templates — create, instantiate, propagate changes |
| 26 | How To Destroy Objects | `Destroy()` method for cleanup, timed destruction |
| 27 | Using GetComponent | `GetComponent<T>()` to access Rigidbody2D, Collider2D, SpriteRenderer at runtime |
| 28 | Boosts & Bumps | Speed boost system using bools, GetComponent, and collision detection |
| 29 | Adding UI Text | TextMeshPro setup — Canvas, TMP import, updating text from code |
| 30 | Wrap Up | Recap of variables, methods, input, collision, prefabs, UI |

**Takeaway:** Extracted usable concepts for DodgeCube — tags for collision detection, booleans for game state, prefabs for obstacles, and UI text for score display.

---

### 26th June 2026 (Thursday)

**Lane B — Build DodgeCube v2 (Main Work)**

Transformed DodgeCube from a rough prototype to a proper mini game.

**Objective 1 — Refactor Existing Code**

Cleaned up the prototype code:
- **`Player.cs`** (now `PlayerController.cs`):
  - Removed dead/unused code from the initial prototype
  - Replaced hardcoded movement speed with a serialized private float
  - Cleaned method naming for clarity
- **Renamed script: `StuffThatNeedsToBeDodged` → `Obstacle.cs`** (finally a sensible name)
- **Fixed bug:** `Random.Range(5f, 4f)` was returning wrong min/max order — arguments were swapped

The player controller now accepts A/D keyboard input, translates the cube horizontally with speed multiplied by deltaTime, and clamps the position using `Mathf.Clamp` against dynamic bounds provided by the GameManager. It only processes input when the game is active.

**Objective 2 — Add Tags**
- Created tag: `Obstacle` in the Unity Tag Manager
- Implemented tag-based collision detection in `Obstacle.cs`:
  - `other.CompareTag("Ground")` → obstacle hit the ground → score!
  - `other.CompareTag("Player")` → player got hit → game over!
- No more generic `OnTriggerEnter2D` — every collision is explicit and intentional.

**Objective 3 — Add Score System**
- Every obstacle that successfully passes the player and hits the ground: **Score +1**
- Score tracked in `GameControll.cs` (later renamed to `GameManager.cs`)
- Score variable is public so `Obstacle.cs` can increment it directly

**Objective 4 — Add UI**
- TextMeshPro score display showing `"Score: 0"`
- Positioned top-left corner of the screen
- Updated via `updateScore()` method that reads the current score and writes to the TMP text component

---

### 27th June 2026 (Saturday)

**Session Stretch 1 — Game State System (Attempt 1)**
- **Start Time:** 3:40 PM
- **End Time:** 10:30 PM (with breaks)

**What was done:**
- Renamed scripts to better reflect their responsibilities
- Pushed current state to GitHub
- Added game state variables (`isGameActive`, `isGameOver`) to support MainMenu and GameOver flows
- Started implementing MainMenu and GameOver logic

**What went wrong:**
- Tried to implement multi-scene logic (separate Menu scene + Game scene)
- Required significant recalibration — references broke across scenes, singleton management was messy
- Cleanup at the end was too complex and error-prone
- **Undid all progress** and reverted to a single-scene approach

**Lesson learned:** Start simple. Single-scene UI toggling is easier to manage than multi-scene navigation at this stage. Will restart fresh.

---

### 28th June 2026 (Sunday)

**Session — New Approach: Single-Scene UI System**
- **Start Time:** 6:15 PM
- **End Time:** 9:10 PM

**Done:**

1. **Dynamic Player Bounds (6:15–6:40 PM)**
   - Replaced hardcoded `moveLimitLeft = -4f` / `moveLimitRight = 4f`
   - Used `Camera.main.ViewportToWorldPoint()` to calculate screen edges in world coordinates
   - Added `playerPadding = 0.5f` so the cube doesn't clip the screen edge

2. **Main Menu UI (Canvas-based, no new scene)**
   - Created a Canvas with:
     - **Title Logo** — "DODGE CUBE" text, styled with a bold font
     - **Game Start Button** — clickable UI button
   - No separate Scene — just panel visibility toggling within the same scene

---

### 29th June 2026 (Monday)

**Session — GameManager, Full Game Loop & GitHub Push**
- **Start Time:** 2:15 PM
- **End Time:** 6:10 PM

**Objective 4 — Create `GameManager.cs`**

Centralized all game logic into a single manager script:

| Responsibility | Implementation |
|---|---|
| Game state | `isGameActive` (bool), `isGameOver` (bool) |
| Score tracking | `score` (int), `finalScore` (int) |
| UI panels | `scorePanel`, `gameOverPanel` (GameObject refs) |
| Player spawning | `SpawnPlayer()` — instantiates `boppyPrefab` at a fixed position |
| Obstacle spawning | Spawns `droppyPrefab` at random X within bounds |
| Dynamic bounds | `moveLimitLeft`, `moveLimitRight` via `ViewportToWorldPoint` |

The `Update()` loop checks if the game is active — if so, it spawns the player on first frame and then spawns obstacles one at a time at random X positions within the dynamic bounds. When the game is over, it calls the method that shows the Game Over panel with the final score.

**Objective 5 — Start Button Logic**
- **On Click:** `GameStart()` sets `isGameActive = true`, shows score panel
- `Update()` loop detects the active state and spawns player + obstacles automatically
- Game does nothing until Start is clicked — clean separation of menu and gameplay

**Objective 6 — Game Over Screen**
- **GameOverPanel** with:
  - "GAME OVER" header text
  - "Final Score: {score}" display (reads from `finalScore`)
  - **Restart button**
- Panel hidden on game start (`SetActive(false)` in `Start()`)
- Shown on player death — hides the score panel, shows the game over panel, copies current score to final score, and resets the game over flag

**Objective 7 — Stop Gameplay on Death**

Three-layer shutdown on collision:
1. **Player** — `PlayerController.Update()` checks `isGameActive` before processing any input
2. **Obstacle** — On collision with Player tag, sets `isGameActive = false` and `isGameOver = true`
3. **Obstacle spawning** — `GameManager.Update()` only spawns when `isGameActive` is true

Player position is clamped using `Mathf.Clamp()` with the dynamic bounds from GameManager.

**Objective 8 — Restart Button (Soft Restart)**
- Resets score and final score to 0
- Calls `GameStart()` again — hides game over panel, shows score panel, re-spawns the player
- No scene reload — just resets all state and starts fresh. Simpler and faster.

**Objective 9 — Final GitHub Push**
- Renamed `BoppyMovement.cs` → `PlayerController.cs`
- Renamed `GameControll.cs` → `GameManager.cs`
- Updated `.gitignore` and pushed all changes

---

### 30th June – 2nd July 2026 (Break — Mouse Failure)

- **Duration:** 3 days
- **Cause:** Mouse developed severe double-clicking issue — single clicks randomly registered as double-clicks, making precise Unity editor work impossible
- **Impact:** Could not effectively select objects, manipulate transforms, or use the Inspector
- **Resolution:** Ordered a replacement mouse

---

### 3rd July 2026 (Friday)

> New mouse arrived. Full steam ahead.

**Session 1 — Unity 2D Course: Lectures 31–40 (Snow Surfer Start)**
- **Start Time:** 3:00 PM
- **End Time:** 5:00 PM

| Lecture | Topic | Key Learning |
|---------|-------|-------------|
| 31 | Section Intro | Overview of Snow Surfer — a side-scrolling physics-based ball game |
| 32 | Game Design | Core mechanics: rolling ball momentum, slopes, obstacles, powerups, finish line |
| 33 | Sprite Shapes | Spline-based 2D terrain — creating slopes, curves, and platforms with Sprite Shape profiles |
| 34 | Edge Colliders | `EdgeCollider2D` conforming to Sprite Shape splines for physics collision surface |
| 35 | Cinemachine Follow | Virtual Camera with damping, look-ahead, and framing for smooth ball following |
| 36 | Character Setup | Ball with Rigidbody2D, parent/child hierarchy |
| 37 | Surface Effector 2D | `SurfaceEffector2D` — applies force to objects touching the surface (slope sliding) |
| 38 | Input System | Unity's modern Input System — `InputAction` assets, key bindings, `Vector2` input values, variable scoping |
| 39 | AddTorque | `Rigidbody2D.AddTorque()` for physics-based ball rotation from input |
| 40 | Finish & Crash | Trigger zones with `OnTriggerEnter2D()` for win/lose detection |

**Session 2 — Hands-On Implementation**
- **Start Time:** 6:30 PM
- **End Time:** 8:30 PM

Built a practice Unity project implementing what I learned:

Wrote a player controller that reads input from the new Input System using `InputSystem.actions.FindAction("Move")`, reads the Vector2 value, and applies `AddTorque` to the Rigidbody2D to rotate the ball left or right.

Created a crash detector that checks the Floor layer using LayerMask and logs a debug message when the player head touches the ground.

Created a finish line script that checks for the Player layer and logs a win message on trigger enter.

Used LayerMask-based detection instead of tags for cleaner, more performant collision checking.

---

### 4th July 2026 (Saturday)

**C# Masterclass — Section 3: Loops**

Worked through loops, arrays, and iterations in C#.

**Concepts covered:**
- `for` loops — counter-controlled iteration
- `foreach` loops — collection iteration without indexing
- Nested loops — loops within loops
- Arrays — single-dimensional and jagged (array of arrays)
- Namespace organization with `namespace Section03`

Exercises completed:
- **CodeExe7** — declared an integer array and printed each element using a `foreach` loop
- **CodeExe8** — built a jagged 2D array with three rows, used nested `for` loops to sum each row and print the totals (output: 6, 15, 24)
- **RocketLanding** — creative console project: a countdown timer from 10 to 0 with ASCII rocket art that descends line-by-line each second using `Thread.Sleep(1000)` and `Console.Clear()` for animation

---

### 5th July 2026 (Sunday)

**C# Masterclass — Section 4: Functions & Methods**

**Concepts covered:**
- Method declaration syntax — access modifiers, return types, parameters
- Passing data into methods via parameters
- Returning values from methods
- Method composition — one method calling another

**CodeExe9 — Temperature Average Calculator:**
Built a program that calculates the average temperature from an array of doubles. Two methods were implemented: `CalculateAverage` which accepts a `double[]` parameter, sums all values with a `foreach` loop, and returns the average; and `PrintAverage` which calls `CalculateAverage` and prints the result to the console. This exercised method parameters of array type, the `return` statement, and method chaining.

---

### 6th July 2026 (Monday)

**Unity 2D Course — Lectures 41–50 (Snow Surfer continued)**

Watched and coded alongside the instructor.

| Lecture | Topic | Implementation |
|---------|-------|----------------|
| 41 | Namespaces & SceneManagement | `SceneManager.LoadScene()` for level transitions |
| 42 | Invoke() For Delays | `Invoke("MethodName", delaySeconds)` — pauses before scene reload after crash |
| 43 | Particle Systems | Created from scratch: emission rate, shape, color-over-lifetime, size-over-lifetime, burst |
| 44 | Triggering Particles | `Play()` / `Stop()` from code |
| 45 | Game Feel Tuning | Tweaked physics values, level layout, added background sprites |
| 46 | FindFirstObjectOfType | `FindAnyObjectByType<SurfaceEffector2D>()` for dynamic boost mechanic |
| 47 | OnCollisionExit2D | Detects when ball leaves ground → stops snow particles |
| 48 | Public Access Modifier | `public bool canControllPlayer` — exposing state for other scripts to disable input |
| 49 | Flip Counting | `Mathf.DeltaAngle()` + `Transform.eulerAngles` to track 360° rotations |
| 50 | Function Parameters | `updateScore(int addScore)` — reusable scoring with parameter |

**Implemented alongside the instructor:**

Updated **CrashDetector** — on floor collision, plays a crash particle effect, calls `CanControllPlayer()` on the player controller to disable input, then uses `Invoke` to wait 1 second before reloading the scene with `SceneManager.LoadScene(0)`.

Updated **FinishLine** — on player collision, plays a finish particle effect and reloads the level after 1 second.

Created **SnowParticleScript** — uses `OnCollisionEnter2D` to play a snow particle effect when the ball touches the floor, and `OnCollisionExit2D` to stop it when airborne. LayerMask-based detection.

Created **ScoreManager** — exposes an `updateScore(int addScore)` method that adds the parameter to the internal score and updates a TextMeshPro text component.

Enhanced **PlayerController** — added flip counting that tracks cumulative rotation using `Mathf.DeltaAngle`. Every time the ball completes a full 360° rotation (past 340° or -340°), it resets the counter and calls `updateScore(100)`. Added a boost mechanic via the Surface Effector's speed property — pressing up increases the surface speed, releasing returns it to base speed. All input is gated by a `canControllPlayer` bool.

---

### 7th July 2026 (Tuesday)

**Unity 2D Course — Lectures 51–59 (Snow Surfer Completed)**

Finished the Snow Surfer section of the course.

| Lecture | Topic | Key Concept |
|---------|-------|-------------|
| 51 | Using Fonts | Importing .ttf, creating TMP Font Asset, applying to score text |
| 52 | ScriptableObjects | Data containers as assets — config data separated from MonoBehaviour |
| 53 | Activating Powerups | Trigger detection → method call → powerup effect applied |
| 54 | Creating a Timer | `Time.deltaTime` countdown in `Update()` for powerup duration |
| 55 | Powerup Particles | Dedicated particle system controlled by powerup state |
| 56 | Anchors & Pivots | UI anchor presets for resolution-independent positioning |
| 57 | Layout Groups | Horizontal/Vertical/Grid Layout Groups for auto-arranging UI |
| 58 | Button OnClick Events | Wiring button clicks in Inspector and in code |
| 59 | Wrap Up | Recap: Input System, particles, ScriptableObjects, access modifiers, function params, UI layout |

**Implemented alongside the instructor:**

Created **PowerupSO** — a ScriptableObject with three serialized fields: power-up type (`"ShortSpeed"` or `"ShortTorque"`), value change (float), and duration (int). Exposes public getter methods for each field.

Created **PowerUpManager** — when the player enters the powerup trigger (detected via LayerMask), the powerup sprite is hidden and the player's activate method is called with the ScriptableObject as an argument. A countdown timer runs each frame using `Time.deltaTime`. When the timer reaches zero, the deactivate method is called, reversing the effect.

Enhanced **PlayerController** with powerup methods — `activatePowerUp` reads the ScriptableObject's type and value, then adds the value to either `baseSpeed`/`boostSpeed` or `moveTorque`. `deactivatePowerUp` subtracts the same values, restoring original stats.

---

### 8th July 2026 (Wednesday)

**Independent Implementation — Snow Surfer From Scratch**

> No walkthrough. No notes. No plan. Just concepts from memory.

Rebuilt the entire Snow Surfer game independently.

**What was implemented:**

| Feature | Implementation |
|---|---|
| **Sprite Shape terrain** | Spline-based slopes and curves with Sprite Shape profile |
| **Edge Colliders** | Conformed to terrain for physics collision |
| **Ball player** | Rigidbody2D with `AddTorque()` rotation |
| **Input System** | `InputSystem.actions.FindAction("Move")` for left/right/up |
| **Surface Effector** | Auto-sliding down slopes, boost on Up arrow |
| **Finish line** | Trigger zone with particle burst + scene reload |
| **Crash detector** | Floor trigger → crash particles → delayed scene reload |
| **Flip counter** | `Mathf.DeltaAngle()` tracking cumulative rotation → score |
| **Snow particles** | `OnCollisionEnter2D`/`OnCollisionExit2D` with LayerMask |
| **ScriptableObject powerups** | Speed boost and torque boost with countdown timer |
| **Score UI** | TextMeshPro with parameterized scoring method |
| **Player control toggle** | Bool flag disables input on crash |

---

## Progress Summary

### C# Masterclass (Denis Panjuta)

| Section | Status | Key Skills |
|---------|--------|------------|
| 1 — Intro, DataTypes & Variables | ✅ Done | Variables, types, conversion, debugging, string manipulation |
| 2 — Making Decisions | ✅ Done | `if/else`, `switch`, ternary, logical operators |
| 3 — Loops | ✅ Done | `for`, `foreach`, `while`, arrays, jagged arrays, nested loops |
| 4 — Functions & Methods | ✅ Done | Method declaration, parameters, return types, method composition |
| 5+ | ⏳ Pending | OOP, Collections, Error Handling, LINQ, Unity sections |

### Unity 2D Game Development (GameDev.tv)

| Section | Lectures | Status | Key Skills |
|---------|----------|--------|------------|
| 1 — Introduction & Setup | 1–6 | ✅ Done | Unity interface, first C# script, GameObject basics |
| 2 — Delivery Dash | 7–30 | ✅ Done | Methods, variables, input, collision, tags, prefabs, GetComponent, UI text |
| 3 — Snow Surfer | 31–59 | ✅ Done | Sprite Shapes, Input System, particles, ScriptableObjects, SceneManagement, Invoke, UI layout |
| 4 — Tilemania | 60–100 | ⏳ Pending | Tilemap, animation, Cinemachine, enemies, coroutines, singletons |
| 5 — Star Blaster | 101–130 | ⏳ Pending | Arrays, loops, waves, health/damage, parallax, AudioManager |

### Projects Built

| Project | Type | Source | Status |
|---------|------|--------|--------|
| **DeliveryDash** | Top-down driving game | Course-taught | ✅ Complete |
| **DodgeCube / BoppyDodge** | 2D dodge game | Self-made from scratch | ✅ Complete (v2 with GameManager) |
| **Snow Surfer** | Side-scrolling physics game | Course-taught + independent rebuild | ✅ Complete (both versions) |
