# Single-Axis-Sidereal-Tracking-Testbed
> A motorised single axis sidereal tracker with software-based tangent-error compensation.
> Experimental characterization of tangent,polar alignment, and mechanical error sources.

**Author:** Rufaida
 **Status:** Planning Phase
**Last Updated:** June 28th, 2026

## Overview
In this project i will use the classic single-arm barn door star tracker as a foundation for an iterative engineering investigation into sidereal tracking performance. Rather than simply replicating an existing design, I will modify the tracker through several iterations, to look into how factors such as tangent error compensation, polar alignment accuracy and mechanical stability affect its ability to track the night sky for long exposure astrophotography. 

## Objectives

- Design and build a single-arm
barn door sidereal tracker using accessible and affordable materials
- Automate the design using an Arduino-compatible microcontroller and stepper motor driver.
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
TK
