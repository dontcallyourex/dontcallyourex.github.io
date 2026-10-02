# dontcallyourex.github.io

Public website of the Don't Call Your Ex app (the app's code is private).

- `/open-this-instead/`: target of the link written into protected contacts.
  Opens the app via Android App Links / iOS Universal Links; without the app
  this page is shown.
- `/privacy/`: privacy policy (linked from the app and the store listings).
- `/.well-known/assetlinks.json`: Android App Links verification. Contains
  the SHA-256 of the signing certificate: debug key now; add the Google Play
  app signing key before release.
- `/.well-known/apple-app-site-association`: iOS Universal Links. Replace
  `TEAMID` with the Apple Developer Team ID in the iOS stage.
- `.nojekyll`: makes GitHub Pages serve the `.well-known` folder.

Plain static files, no build step.
