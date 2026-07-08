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

- **Platform:** Udemy
- **Instructor:** Denis Panjuta
- **Duration:** 46h 12m · 484 lectures · 28 sections
- **URL:** https://www.udemy.com/share/1013Gg/
- **Code Repo:** `/mnt/fast/C#`

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
- **Guide:** `/mnt/storage1/OpenCode to Rescue/Complete_CSharp_Unity_2D_Course_Guide.md`

| Section | Lectures | Status | Date Completed |
|---------|----------|--------|----------------|
| 1 — Introduction & Setup | 1–6 | Done | 19th June |
| 2 — Delivery Dash | 7–30 | Done | 25th June |
| 3 — Snow Surfer | 31–59 | Done | 7th July |
| 4 — Tilemania | 60–100 | Pending | — |
| 5 — Star Blaster | 101–130 | Pending | — |

---

## Projects

### DodgeCube (`/mnt/storage1/Projects/DodgeCube`)

- **Repository:** [Ishit-Parikh/DodgeCube](https://github.com/Ishit-Parikh/DodgeCube)
- **Unity Version:** 6000.3.18f1
- **Type:** Self-made 2D dodge game (no tutorial)
- **Scripts:** `GameManager.cs`, `PlayerController.cs`, `Obstacle.cs`

### Snow Surfer Practice (`/mnt/storage1/Projects/UNITY2D Course Learning Section - 2`)

- **Type:** Course-taught game + independent rebuild
- **Scripts:** `PlayerController.cs`, `ScoreManager.cs`, `CrashDetector.cs`, `FinishLine.cs`, `SnowParicleScript.cs`, `PowerUpManager.cs`, `PowerupSO.cs`

### DeliveryDash Practice (`/mnt/storage1/Projects/UNITY 2D Course Learnings`)

- **Type:** Course-taught practice
- **Scripts:** `Movement.cs`, `Delivery.cs`

### C# Masterclass Code (`/mnt/fast/C#`)

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
  - Replaced hardcoded movement speed with `[SerializeField] private float moveSpeed`
  - Cleaned method naming for clarity
- **Renamed script: `StuffThatNeedsToBeDodged` → `Obstacle.cs`** (finally a sensible name)
- **Fixed bug:** `Random.Range(5f, 4f)` was returning wrong min/max order → corrected to `Random.Range(-4f, 4f)`

**Script: `PlayerController.cs`**
```csharp
[SerializeField] private float moveSpeed = 2.5f;
private GameManager _gameManager;

void Start()
{
    _gameManager = Object.FindAnyObjectByType<GameManager>();
}

void Update()
{
    if (_gameManager.isGameActive)
    {
        float move = 0f;
        if (Keyboard.current.aKey.isPressed) move = -7.5f;
        else if (Keyboard.current.dKey.isPressed) move = 7.5f;

        transform.Translate(move * moveSpeed * Time.deltaTime, 0, 0);

        Vector3 pos = transform.position;
        pos.x = Mathf.Clamp(pos.x, _gameManager.moveLimitLeft, _gameManager.moveLimitRight);
        transform.position = pos;
    }
}
```

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

   ```csharp
   moveLimitLeft = Camera.main.ViewportToWorldPoint(new Vector3(0, 0, 0)).x + playerPadding;
   moveLimitRight = Camera.main.ViewportToWorldPoint(new Vector3(1, 0, 0)).x - playerPadding;
   ```

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
| Player spawning | `SpawnPlayer()` — instantiates `boppyPrefab` at `(0, -2.295, 0)` |
| Obstacle spawning | Spawns `droppyPrefab` at random X within bounds |
| Dynamic bounds | `moveLimitLeft`, `moveLimitRight` via `ViewportToWorldPoint` |

**`GameManager.Update()` flow:**
```csharp
void Update()
{
    if (isGameActive)
    {
        if (!isPlayerSpawned) SpawnPlayer();
        else if (!isObstacleSpawned)
        {
            xPostion = Random.Range(moveLimitLeft, moveLimitRight);
            Instantiate(droppyPrefab, new Vector3(xPostion, 0, 0), Quaternion.identity);
            isObstacleSpawned = true;
        }
    }
    else if (isGameOver)
    {
        GameOverPanel();
    }
}
```

**Objective 5 — Start Button Logic**
- **On Click:** `GameStart()` sets `isGameActive = true`, shows score panel
- `Update()` loop detects the active state and spawns player + obstacles automatically
- Game does nothing until Start is clicked — clean separation of menu and gameplay

**Objective 6 — Game Over Screen**
- **GameOverPanel** with:
  - "GAME OVER" header text
  - "Final Score: {score}" display (reads from `finalScore`)
  - **Restart button**
- Panel hidden on game start (`gameOverPanel.SetActive(false)` in `Start()`)
- Shown via `GameOverPanel()` method on player death:
  ```csharp
  void GameOverPanel()
  {
      scorePanel.SetActive(false);
      gameOverPanel.SetActive(true);
      finalScore = score;
      FinalSocreText.text = "Final Score: " + finalScore.ToString();
      isGameOver = false;
  }
  ```

**Objective 7 — Stop Gameplay on Death**

Three-layer shutdown on collision:
1. **Player** — `PlayerController.Update()` checks `isGameActive` before processing any input
2. **Obstacle** — `Obstacle.OnTriggerEnter2D()` with Player tag sets `isGameActive = false` and `isGameOver = true`
3. **Obstacle spawning** — `GameManager.Update()` only spawns when `isGameActive` is true

Player position is clamped using `Mathf.Clamp()` with the dynamic bounds from GameManager.

**Objective 8 — Restart Button (Soft Restart)**
```csharp
public void RestartGame()
{
    score = 0;
    updateScore();
    finalScore = 0;
    GameStart();  // hides gameOverPanel, shows scorePanel, re-spawns player
}
```
No scene reload — just resets all state and calls `GameStart()` again. Simpler and faster.

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

**`PlayerController.cs` (Snow Surfer version):**
```csharp
private InputAction moveAction;
private Rigidbody2D _rigidbody2D;

void Start()
{
    moveAction = InputSystem.actions.FindAction("Move");
    _rigidbody2D = GetComponent<Rigidbody2D>();
}

void Update()
{
    Vector2 moveVector = moveAction.ReadValue<Vector2>();
    if (moveVector.x < 0) _rigidbody2D.AddTorque(moveTorque);
    else if (moveVector.x > 0) _rigidbody2D.AddTorque(-moveTorque);
}
```

**`CrashDetector.cs`:**
```csharp
void OnTriggerEnter2D(Collider2D other)
{
    int layerIndex = LayerMask.NameToLayer("Floor");
    if (other.gameObject.layer == layerIndex)
    {
        Debug.Log("Player head is touching the ground.");
    }
}
```

**`FinishLine.cs`:**
```csharp
void OnTriggerEnter2D(Collider2D other)
{
    int layerIndex = LayerMask.NameToLayer("Player");
    if (other.gameObject.layer == layerIndex)
    {
        Debug.Log("Player has won the game.");
    }
}
```

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

**`CodeExe7.cs` — foreach loop:**
```csharp
int[] myInts = new int[5];
myInts = new int[] {1, 2, 3, 4, 5};
foreach(int ints in myInts)
{
    System.Console.WriteLine(ints);
}
```

**`CodeExe8.cs` — nested for loops with jagged 2D array:**
```csharp
int[][] my2Darray =
{
    new int[] {1, 2, 3},
    new int[] {4, 5, 6},
    new int[] {7, 8, 9}
};
for (int i = 0; i < my2Darray.Length; i++)
{
    int sum = 0;
    for (int j = 0; j < my2Darray[i].Length; j++)
    {
        sum += my2Darray[i][j];
    }
    Console.WriteLine(sum);
}
// Output: 6, 15, 24
```

**`RocketLanding.cs` — creative project:**
```csharp
string RocketLanding = "   /\\\n  /  \\\n /____\\\n   ||\n   ||\n   VV";
for (int i = 10; i >= 0; i--)
{
    Console.Clear();
    System.Console.WriteLine($"Counter: {i}");
    System.Console.WriteLine(RocketLanding);
    RocketLanding = "\r\n" + RocketLanding;
    Thread.Sleep(1000);
}
System.Console.WriteLine("Rocket has landed successfully.");
```
A countdown timer (10 → 0) with ASCII rocket art that descends the terminal, using `Thread.Sleep(1000)` for 1-second intervals and `Console.Clear()` for animation frames.

---

### 5th July 2026 (Sunday)

**C# Masterclass — Section 4: Functions & Methods**

**Concepts covered:**
- Method declaration syntax — access modifiers, return types, parameters
- Passing data into methods via parameters
- Returning values from methods
- Method composition — one method calling another

**`CodeExe9.cs` — Temperature Average Calculator:**

The challenge: Create a program that calculates average temperature from an array of doubles.

```csharp
public class CodeExe9
{
    static double[] temps = {23.5, 23.5, 23.5, 23.5, 23.5, 23.5, 23.5, 23.5, 23.5, 23.5};

    public static void Run()
    {
        PrintAverage(temps);
    }

    public static double CalculateAverage(double[] temperatures)
    {
        double tempSum = 0;
        foreach (double temp in temperatures)
        {
            tempSum += temp;
        }
        return tempSum / temperatures.Length;
    }

    public static void PrintAverage(double[] temperatures)
    {
        System.Console.WriteLine($"The Average Temperature is: {CalculateAverage(temperatures)}");
    }
}
```

**Key patterns exercised:**
- Method parameter of array type (`double[]`)
- `foreach` loop to accumulate values
- `return` statement to pass computed value back to caller
- Method chaining — `PrintAverage()` calls `CalculateAverage()` internally

---

### 6th July 2026 (Monday)

**Unity 2D Course — Lectures 41–50 (Snow Surfer continued)**

Watched and coded alongside the instructor.

| Lecture | Topic | Implementation |
|---------|-------|----------------|
| 41 | Namespaces & SceneManagement | `using UnityEngine.SceneManagement;` — `SceneManager.LoadScene()` for level transitions |
| 42 | Invoke() For Delays | `Invoke("MethodName", delaySeconds)` — pauses before scene reload after crash |
| 43 | Particle Systems | Created from scratch: emission rate, shape, color-over-lifetime, size-over-lifetime, burst |
| 44 | Triggering Particles | `particleSystem.Play()` / `particleSystem.Stop()` from code |
| 45 | Game Feel Tuning | Tweaked physics values, level layout, added background sprites |
| 46 | FindFirstObjectOfType | `FindAnyObjectByType<SurfaceEffector2D>()` for dynamic boost mechanic |
| 47 | OnCollisionExit2D | Detects when ball leaves ground → stops snow particles |
| 48 | Public Access Modifier | `public bool canControllPlayer` — exposing state for other scripts to disable input |
| 49 | Flip Counting | `Mathf.DeltaAngle()` + `Transform.eulerAngles` to track 360° rotations |
| 50 | Function Parameters | `updateScore(int addScore)` — reusable scoring with parameter |

**Implemented alongside the instructor:**

**`CrashDetector.cs` (updated — full version):**
```csharp
[SerializeField] private ParticleSystem crashParticleSystem;
PlayerController _playerController;

void Start()
{
    _playerController = FindAnyObjectByType<PlayerController>();
}

void OnTriggerEnter2D(Collider2D other)
{
    int layerIndex = LayerMask.NameToLayer("Floor");
    if (other.gameObject.layer == layerIndex)
    {
        crashParticleSystem.Play();          // Show crash particles
        _playerController.CanControllPlayer(); // Disable player input
        Invoke("SceneReload", 1);             // Wait 1s, then reload
    }
}

void SceneReload()
{
    SceneManager.LoadScene(0);
}
```

**`FinishLine.cs` (updated — full version):**
```csharp
[SerializeField] private ParticleSystem finishLineParticleSystem;

void OnTriggerEnter2D(Collider2D other)
{
    int layerIndex = LayerMask.NameToLayer("Player");
    if (other.gameObject.layer == layerIndex)
    {
        finishLineParticleSystem.Play();
        Invoke("SceneReload", 1);
    }
}

void SceneReload() => SceneManager.LoadScene(0);
```

**`SnowParicleScript.cs` — snow trail effect:**
```csharp
[SerializeField] private ParticleSystem snowParticleSystem;

private void OnCollisionEnter2D(Collision2D other)
{
    int LayerIndex = LayerMask.NameToLayer("Floor");
    if (other.gameObject.layer == LayerIndex)
        snowParticleSystem.Play();
}

private void OnCollisionExit2D(Collision2D other)
{
    int LayerIndex = LayerMask.NameToLayer("Floor");
    if (other.gameObject.layer == LayerIndex)
        snowParticleSystem.Stop();
}
```

**`ScoreManager.cs` — parameterized scoring:**
```csharp
[SerializeField] private TextMeshProUGUI scoreText;
private int score = 0;

public void updateScore(int addScore)
{
    score += addScore;
    scoreText.text = "Score: " + score.ToString();
}
```

**`PlayerController.cs` — enhanced with flip counting and boosting:**
```csharp
void Update()
{
    if (canControllPlayer)
    {
        rotatePlayer();
        boostPlayer();
        flipCounts();
    }
}

void flipCounts()
{
    float currentRotation = transform.rotation.eulerAngles.z;
    totalRotation += Mathf.DeltaAngle(previousRotation, currentRotation);
    if (totalRotation > 340 || totalRotation < -340)
    {
        totalRotation = 0;
        _scoreManager.updateScore(addScore);  // +100 points per full flip
    }
    previousRotation = currentRotation;
}

void boostPlayer()
{
    moveVector = moveAction.ReadValue<Vector2>();
    if (moveVector.y > 0)
        _surfaceEffector2D.speed = boostSpeed;  // Up arrow = faster slope
    else
        _surfaceEffector2D.speed = baseSpeed;
}
```

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

**`PowerupSO.cs` — ScriptableObject for powerup data:**
```csharp
[CreateAssetMenu(fileName = "PowerupSO", menuName = "Scriptable Objects/PowerupSO")]
public class PowerupSO : ScriptableObject
{
    [SerializeField] private string powerUpType;   // "ShortSpeed" or "ShortTorque"
    [SerializeField] private float valueChange;     // Amount to modify
    [SerializeField] private int time;              // Duration in seconds

    public string GetPowerUpType() => powerUpType;
    public float GetValueChange() => valueChange;
    public int GetTime() => time;
}
```

**`PowerUpManager.cs` — pickup logic with countdown timer:**
```csharp
[SerializeField] private PowerupSO _powerupSo;
private PlayerController _playerController;
private SpriteRenderer _spriteRenderer;
private float timeLeft;

void Start()
{
    _playerController = FindAnyObjectByType<PlayerController>();
    _spriteRenderer = FindAnyObjectByType<SpriteRenderer>();
    timeLeft = _powerupSo.GetTime();
}

void Update() => CountDownTimer();

void CountDownTimer()
{
    if (!_spriteRenderer.enabled)  // Powerup was collected (sprite hidden)
    {
        if (timeLeft > 0)
        {
            timeLeft -= Time.deltaTime;
            if (timeLeft <= 0)
                _playerController.deactivatePowerUp(_powerupSo);
        }
    }
}

void OnTriggerEnter2D(Collider2D other)
{
    int LayerIndex = LayerMask.NameToLayer("Player");
    if (other.gameObject.layer == LayerIndex && _spriteRenderer.enabled)
    {
        _spriteRenderer.enabled = false;
        _playerController.activatePowerUp(_powerupSo);
    }
}
```

**`PlayerController.cs` — powerup activation/deactivation:**
```csharp
public void activatePowerUp(PowerupSO powerupSo)
{
    if (powerupSo.GetPowerUpType() == "ShortSpeed")
    {
        baseSpeed += powerupSo.GetValueChange();
        boostSpeed += powerupSo.GetValueChange();
    }
    else if (powerupSo.GetPowerUpType() == "ShortTorque")
    {
        moveTorque += powerupSo.GetValueChange();
    }
}

public void deactivatePowerUp(PowerupSO powerupSo)
{
    if (powerupSo.GetPowerUpType() == "ShortSpeed")
    {
        baseSpeed -= powerupSo.GetValueChange();
        boostSpeed -= powerupSo.GetValueChange();
    }
    else if (powerupSo.GetPowerUpType() == "ShortTorque")
    {
        moveTorque -= powerupSo.GetValueChange();
    }
}
```

---

### 8th July 2026 (Wednesday)

**Independent Implementation — Snow Surfer From Scratch**

> No walkthrough. No notes. No plan. Just concepts from memory.

Rebuilt the entire Snow Surfer game independently in the `UNITY2D Course Learning Section - 2` project.

**What was implemented:**

| Feature | Implementation |
|---|---|
| **Sprite Shape terrain** | Spline-based slopes and curves with Sprite Shape profile |
| **Edge Colliders** | Conformed to terrain for physics collision |
| **Ball player** | Rigidbody2D with `AddTorque()` rotation |
| **Input System** | `InputSystem.actions.FindAction("Move")` for left/right/up |
| **Surface Effector** | Auto-sliding down slopes, boost on Up arrow |
| **Finish line** | Trigger zone with particle burst + `SceneManager.LoadScene(0)` |
| **Crash detector** | Floor trigger → crash particles → `Invoke("SceneReload", 1)` |
| **Flip counter** | `Mathf.DeltaAngle()` tracking cumulative rotation → score |
| **Snow particles** | `OnCollisionEnter2D`/`OnCollisionExit2D` with LayerMask |
| **ScriptableObject powerups** | Speed boost and torque boost with countdown timer |
| **Score UI** | TextMeshPro with parameterized `updateScore(int)` |
| **Player control toggle** | `canControllPlayer` bool disables input on crash |

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
| **Snow Surfer** | Side-scrolling physics ball game | Course-taught + independent rebuild | ✅ Complete (both versions) |
