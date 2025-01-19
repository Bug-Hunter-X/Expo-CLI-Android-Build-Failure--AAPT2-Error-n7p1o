# Expo CLI Android Build Failure: AAPT2 Error

This repository demonstrates a common yet elusive error encountered when building Android APKs using the Expo CLI. The build process abruptly terminates with a generic "AAPT2 error," leaving developers with insufficient information for debugging.

## Problem Description

The issue manifests as a failed build, usually accompanied by an unhelpful error message within the Android build logs.  This makes identifying the root cause extremely difficult.

## Reproduction Steps

1. Clone this repository.
2. Install the required dependencies: `npm install` or `yarn install`
3. Attempt to build the Android APK using `expo build:android`.
4. Observe the AAPT2 error in the build logs.

## Solution

The provided solution demonstrates a potential fix.  It involves inspecting resource files (images, layouts, etc.) for potential issues like invalid XML or missing resources, and thoroughly cleaning the project cache.  Examine the `bugSolution.js` file for implementation details.