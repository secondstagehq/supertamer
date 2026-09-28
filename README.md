# Supertamer

A product-building companion for people who build alone — a native macOS app.

This repository distributes beta builds. Get the newest one from
[Releases](https://github.com/secondstagehq/supertamer/releases).

**The app's source is not public.** GitHub attaches a "Source code" archive to every release
automatically; here that archive is this README and nothing else.

## Requirements

- macOS 14 or later
- Apple Silicon (the app is built and tested on Apple Silicon only)

## Install

1. Download the `Supertamer-*.zip` asset from the newest release and unzip it.
2. Move `Supertamer.app` to `/Applications`, replacing any older copy of the same name.
3. Open it. Builds are signed with a Developer ID certificate and notarized by Apple, so
   Gatekeeper should not warn you and no `xattr` workaround is needed.
4. If you keep agent sessions open, restart them after installing — a running session keeps
   talking to the helper binary it started with.

### Upgrading from a build older than 2026-08-31

Earlier betas installed two apps side by side. The transition is over and there is one app now,
so delete the retired one by hand — a new install replaces `Supertamer.app` only, and leaving the
old bundle in place lets it compete for `supertamer://` links:

```bash
rm -rf /Applications/SupertamerWeb.app
```

Your data is untouched by this. Both bundles opened the same local database and the same iCloud
container, and settings you changed in the newer shell are carried over on first launch.

## Beta expiry

Each beta carries a signed expiry date and refuses to open your data after it. The current build
expires **2026-11-01 00:00 UTC**. Expiring changes nothing in your database — install a newer
build and it opens again.

## Support

Report problems in [Issues](https://github.com/secondstagehq/supertamer/issues).
