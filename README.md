# Duplicate Firebase App Initialization Bug
This repository demonstrates a common error encountered when working with Firebase: attempting to initialize the Firebase app multiple times.  The error message typically reads:  `FirebaseError: Firebase App named '[DEFAULT]' already exists or has been created during initialization.`

The `bug.js` file shows the erroneous code, while `bugSolution.js` provides the corrected version. This issue often arises when multiple parts of your application inadvertently try to initialize Firebase, leading to conflicts.

**Solution:** Ensure Firebase is initialized only once in your application, typically in a central location (e.g., at the entry point of your application).