# Single-Axis-Sidereal-Tracking-Testbed
> A motorised single axis sidereal tracker with software-based tangent-error compensation.
> Experimental characterization of tangent,polar alignment, and mechanical error sources.

**Author:** Rufaida
 **Status:** Planning Phase
**Last Updated:** July 10th, 2026

## Overview
In this project i will use the classic single-arm barn door star tracker (inspired by [George Haig's design](https://en.wikipedia.org/wiki/Barn_door_tracker)) as a foundation for an iterative engineering investigation into sidereal tracking performance. Rather than simply replicating an existing design, I will modify the tracker through several iterations, to look into how factors such as tangent error compensation, polar alignment accuracy and mechanical stability affect its ability to track the night sky for long exposure astrophotography. 

## Objectives

- Design and build a single-arm
barn door sidereal tracker using accessible and affordable materials
- Automate the design using an Arduino-compatible microcontroller and stepper motor driver.
- Make a calculator to output the optimum constant speed.
- Establish a baseline by evaluating constant-speed sidereal tracking performance.
- Derive the theoretical tangent error of a tangent-arm tracker and predict the exact star trailing at constant speed.
- Validate the derivation experimentally by taking constant-speed photos and measuring the actual star trails.
Compare theory to reality.
- Investigate, quantify and minimize discrepancies** by refining polar alignment, reducing mechanical backlash, and tightening structural flexure without changing the motor speed.
- Characterize the system's sensitivity to polar alignemnt to determine the alignment accuracy required for 3-minute exposures at 50mm.
- Develop a simple  tool that calculates step delay tables for any user's hinge length and rod pitch.
- Implement software-based tangent compensation** using motor speed correction, and demonstrate that the remaining tangent error is eliminated.
- Compare constant-speed tracking with
tangent-error-compensated tracking to
determine the practical impact of tangent
error.
- Validate the completed tracker through
long-exposure DSLR astrophotography.
- Document the complete design, development, and experimental process.



## Experimental Phases
| Phase | Research Question | Expected Outcome |
|---|---|---|
| **0. Theoretical Model** | What tracking error should an ideal tangent-arm tracker exhibit? | Mathematical model of tangent error and predicted star trailing. |
| **1. Engineering Validation** | Is the tracker mechanically and electronically reliable enough for experimentation? | Verified operation of the motor, electronics, and mechanical drive system. |
| **2. Baseline Tracking** | How accurately does a constant-speed tangent-arm tracker follow the night sky? | Baseline tracking performance compared with theoretical predictions. |
| **3. Residual Error Analysis** | Why does the measured tracking error differ from the theoretical prediction? | Identification of the dominant sources of tracking error. |
| **4. Mechanical Investigation** | How much do mechanical improvements reduce total tracking error? | Quantitative comparison of tracking performance before and after mechanical modifications. |
| **5. Polar Alignment Investigation** | How does the accuracy of polar alignment influence tracking performance? | Comparison of different alignment methods and their effect on maximum usable exposure time. |
| **6. Tangent-Error Compensation** | How much does software-based tangent-error compensation improve tracking accuracy? | Direct comparison between constant-speed and compensated tracking. |
| **7. Final Validation** | What is the maximum achievable performance of the optimized tracker? | Final tracking accuracy, exposure limits, and comparison with theoretical expectations. |
| **8. Astrophotography Demonstration** | What imaging performance can the completed system achieve under dark skies? | Final processed astrophotographs captured with the completed tracker. |


## 🧮 Calculator & Theoretical Mathematics

Because straight-rod barn door trackers suffer from tangent error, a constant motor speed will inevitably cause tracking drift over long exposures. However, for those of you who do not want to go the extra mile, and plan on sticking to shorter exposures, this calculator can help find the optimum motor speed for you.

* **[Launch the Live Interactive Calculator](https://rufaida19-sys.github.io/Single-Axis-Sidereal-Tracking-Testbed/calculator/calculator.html)** - Input your tracker's physical dimensions to get your optimized motor RPM.
*  **[Read the Full Mathematical Derivation](./calculator/THEORY.md)** - A deep dive into the calculus, angular error functions, and the equioscillation principle used to solve this problem.
