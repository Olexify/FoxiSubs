# Privacy Policy

**Kitsumi browser extension**
Last updated: 2 September 2026

## Summary

Kitsumi has no accounts, no servers, and no analytics. Everything it stores,
it stores in your own browser. It makes network requests only when you use a
feature that needs one, and every one of those is listed below.

## What Kitsumi stores, and where

All of the following is kept locally in your browser, using extension storage
and IndexedDB. None of it is transmitted anywhere.

- Your settings: subtitle appearance, position, timing offsets, per-show sync
  offsets, interface preferences, allowlisted sites.
- Your study data: words you have looked up, words marked as known, study
  time, streaks, active days, ranks and achievements, per-language statistics.
- Dictionaries you install, stored as local databases.
- Subtitle files you load, for the duration of playback.
- API keys you choose to enter for optional third-party services.

You can delete all of it at any time by removing the extension, or by using
the reset controls in the extension's settings.

## When Kitsumi makes network requests

Kitsumi does not contact any server operated by the developer, because none
exists. It contacts third-party services only in response to an action you
take:

| You do this | Kitsumi contacts | What is sent |
| :--- | :--- | :--- |
| Search for subtitles | Jimaku, OpenSubtitles, SubDL, Kitsunekko | The title or search terms you typed |
| Download a dictionary | GitHub Releases, Hugging Face and other hosts listed in the dictionary catalog | A file request. No personal data |
| Look up a word externally | The dictionary site you selected | The word you looked up |
| Enable AI definitions (optional) | Groq | The word or sentence being processed, plus your own Groq API key |
| Enable AI imagery (optional) | WaveSpeed | The prompt text, plus your own WaveSpeed API key |
| Mine a card to Anki | AnkiConnect on `http://localhost:8765` | The card contents. This request never leaves your computer |

The AI features are off by default and stay dormant until you enter your own
API key. With no key present, no request is made to Groq or WaveSpeed at any
time.

Each third-party service handles the data it receives under its own privacy
policy. If you enable an AI feature, you are choosing to send that content to
that provider under your own account.

## Subtitle search keys

Jimaku search works on first run using a shared, rate-limited API key bundled
with the extension. It is there so you can try subtitle search immediately
without signing up for anything. It is not tied to you and identifies nothing
about you.

**The shared key is for initial testing only.** It is rate-limited across
everyone using the extension, so for regular use you should get your own free
Jimaku key and enter it in settings.

## Site access

Kitsumi requests access to all sites because subtitles have to be rendered
over video players it cannot know about in advance, including players inside
embedded frames. It reads page content only to locate the video player and
its subtitle track, and only on pages where you use it or that you have
allowlisted.

Kitsumi does not read, collect, or transmit the contents of pages you visit.

If you would rather narrow this, both browsers let you restrict an extension
to specific sites:

- **Chrome:** right-click the extension icon, "This can read and change site
  data", "On specific sites".
- **Firefox:** Add-ons Manager, Kitsumi, Permissions.

All features continue to work on the sites you allow.

## What Kitsumi never does

- No user accounts, sign-in, or registration.
- No analytics, telemetry, crash reporting, or usage tracking.
- No advertising and no advertising identifiers.
- No selling or sharing of data, because none is collected.
- No transmission of your study history, vocabulary, or statistics anywhere.

## Children

Kitsumi is a general-purpose study tool and does not knowingly collect data
from anyone, including children.

## Changes

Material changes to this policy will be published in this file, and its
"last updated" date will change. The version history is public in this
repository.

## Contact

Questions about this policy: olexifyyy@gmail.com
Or ask in the [Discord](https://discord.gg/UpmNHxT7PF).
