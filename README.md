# Paper Management Assistant

This project uses Firebase for authentication and data storage.

## Setup

1. Copy `firebase-config-example.js` to `firebase-config.js` and replace the placeholder values with your Firebase project credentials.
   Keep `firebase-config.js` out of version control (see `.gitignore`).

   ```bash
   cp firebase-config-example.js firebase-config.js
   ```

2. Deploy the Firestore security rules in `firestore.rules` using the Firebase CLI:

   ```bash
   firebase deploy --only firestore:rules
   ```

   You can also test them locally with the emulator:

   ```bash
   firebase emulators:exec --project <project-id> "npm test"
   ```
