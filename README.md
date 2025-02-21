# Expo EAS Build Failure: Silent Native Module Errors

This repository demonstrates a common yet often elusive bug in Expo's EAS Build system.  The issue involves a failure to properly link or handle native modules, resulting in cryptic error messages or silent build failures.  The challenge lies in pinpointing the exact source of the problem.

## Reproducing the Issue
The `bug.js` file contains a simplified example.  You'll need to configure a project that relies on a native module and trigger a build via EAS Build.  The build will fail.  Note that the error message is often unhelpful, making debugging challenging.

## Solution
The `bugSolution.js` shows how to correctly integrate native module dependencies for EAS Build.  This often involves meticulously reviewing your native module setup (including Android and iOS configurations) and ensuring the required native modules are properly linked and configured in your project's build settings.