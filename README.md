# Expo Android Build Failure: Cryptic Package Name Error

This repository demonstrates a bug encountered when building an Android app using Expo CLI. The issue involves a mismatch in package names defined in `app.json` and the actual Android project configuration.  The iOS build works correctly, but the Android build fails with an unhelpful error message.

## Problem

The problem lies in the inconsistency between the package name specified in `app.json` (under `expo.android.package`) and the package name used in the Android project itself. This mismatch leads to a build failure during the Android build process. The error message is not very informative, making it challenging to identify the root cause.

## Solution

The solution involves verifying and ensuring the consistency of the package name across both the `app.json` configuration and the actual Android project settings. This typically involves correcting the `expo.android.package` name in `app.json` to accurately reflect the project's package name.

## Reproduction Steps

1. Clone this repository.
2. Navigate to the project directory.
3. Try building the Android app using `expo build:android`. Observe the error.
4. Apply the solution and rebuild the app.