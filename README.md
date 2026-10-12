# MyCar

The car from the Vehicle Systems & Components hands-on session, finished: every component
from hands-on steps 01–10, with its tests. Lecture 1 starts from here and puts a cruise
controller in front of `Car`.

## Get your own copy

1. **Use this template → Create a new repository**, name it `MyCar`, owner: you.
2. In VS Code: **Git: Clone** your new repository and open the folder.
3. Dyad Studio runs `Pkg.instantiate()` by itself. The first time it downloads and
   precompiles the libraries — minutes, not seconds.
4. Status bar, bottom left: `main` → **Create new branch…** → `lecture-01`. The lecture goes
   on that branch.

Keep the name `MyCar`: the lecture's plot commands start with `using MyCar, Plots; plotly()`.

## What is in it

| Component | Hands-on step | What it is |
| --- | --- | --- |
| `Engine`, bench `EngineStep` | 02 | torque command in, shaft torque out: delay, lag, 150 N·m ceiling |
| `Driveline` | 03 | gear and rolling wheel |
| `Body` | 04 | mass, air drag, rolling resistance |
| `Car`, bench `CarFullThrottle` | 05 | torque command in, speed in km/h out — 246 km/h flat out |
| `WheeledDriveline`, `WheeledCar` | 06 | the same car with wheel inertia |
| `GradeForce`, `GradeBody` | 07 | the body on a hill, with a `grade` input |
| `TireFrictionCurve` | 08 | grip against slip |
| `SlipWheel1D` | 09 | a wheel that can spin |
| `SlipCar`, bench `SlipCarStandingStart` | 10 | wheelspin on ice |

Each component has a test case; run them all with `]` → `test` in the Julia REPL.

## Course pages

- Hands-on guide: <https://dr14-make.github.io/16ESPD/handson/lecture-01/>
- Lecture 1 build guide: <https://dr14-make.github.io/16ESPD/lecture/lecture-01/>
