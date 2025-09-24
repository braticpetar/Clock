# Unity Analog Clock

A very simple Unity project based on the [Catlike Coding tutorial](https://catlikecoding.com/unity/tutorials/basics/game-objects-and-scripts/)

![GIF](Assets/clock.gif)

## Features
- Project is used to demonstrate some of the Unity's basic concepts:
  - GameObjects and Transforms
  - Custom scripts
  - Quaternion rotations

## How It Works
- Each clock hand is a child of it's pivot point, so the hands rotate around the clock center instead of their own center point
- We get TimeSpan from `DateTime.Now.TimeOfDay`
- Time values are converted into degrees:
  - Hours × -30°
  - Minutes × -6°
  - Seconds × -6°
- Rotations are applied using `Quaternion.Euler`


