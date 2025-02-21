# Inconsistent Dimensions on Android in React Native

This repository demonstrates a common but elusive bug in React Native's `Dimensions` API on Android.  The issue involves the inconsistent or incorrect return of screen dimensions using `Dimensions.get('window')` or `Dimensions.get('screen')`. The bug can manifest as dimensions smaller than expected, completely incorrect values, or even zeros.

This issue is particularly problematic because it's often intermittent, making it difficult to reproduce consistently and leading to frustrating debugging sessions.

The repository includes example code illustrating the problem and a proposed solution.

## Bug Reproduction

To reproduce the bug:

1. Clone this repository.
2. Run the app on an Android device or emulator.
3. Observe the logged dimensions.  Note that they might not always be correct, and may vary between runs or orientation changes. 

## Solution

The solution involves using a combination of `Dimensions` along with techniques to ensure the values are correct and handle any inconsistencies reliably.