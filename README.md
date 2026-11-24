# AppList Catalog.

This repository is an open-source collection of popular iOS apps with known Universal Links & URL Schemes.

The list is directly used by AppList, a FREE minimalist app launcher for iPhone that also respects your privacy (no tracking, no ads):
- https://sxp.studio/applist

<img src="./app-list.jpg" alt="AppList. Screenshot" width="320" />

# Contributing

Contributions are welcome! 

Requirements:
1. Valid App Name
2. Valid Universal Link (preferred) or URL Scheme 
3. Your URL must open the app in a default state (i.e. not start some unexpected action like initiate a call with someone)

Nice to have (but accelerate the approval):
4. Video recording showing that your URL works

Once approved and merged, all you will need to do is restart your app for it to pick up the latest version.

## Bundle identifiers

The optional `bundleID` field identifies the iOS app itself. Preserve capitalization and use the identifier for the same regional app as the catalog URL. The catalog's `id` is a separate, stable key used by saved AppList selections.

For App Store apps, look up the numeric ID from the listing in its storefront and copy the returned `bundleId`. For built-in apps, Apple publishes the identifiers directly. [Example App Store lookup](https://itunes.apple.com/lookup?id=335948517&country=it) · [Apple’s list of iPhone and iPad bundle IDs](https://support.apple.com/guide/deployment/depece748c41/web)

# Special Cases

Below is a *non-exhaustive* list of apps purposedly not included in the official list:

**Facetime**:
- Reason: Require an argument & automatically start a call
- URL Scheme: `facetime://[phone-or-email]`

# License

MIT License.

