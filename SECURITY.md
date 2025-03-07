# Reporting a vulnerability

Report security vulnerabilities to [security@turbowarp.org](mailto:security@turbowarp.org) instead of the public issue tracker.

If you don't get a response within 48 hours, post a GitHub issue asking for an update. It may have been flagged as spam. (do not post any details publicly, just ask if your email was seen)

## Bug Bounty

<!-- Inspired by the SerenityOS bug bounty program: https://serenityos.org/bounty/ -->

We don't have a large budget, but we take security very seriously. I will pay out a bug bounty **starting at $20 USD** for high severity bugs like these (non-comprehensive):

 - XSS in places such as the compiler or any extension in the [official extension gallery](https://extensions.turbowarp.org/) (including unlisted ones)
 - Sandbox escape in the desktop app (such as arbitrary file read/write) assuming that XSS has already been achieved (so running any code in developer tools is fair game)
 - Code execution/memory corruption/etc. on any of our backend services

These types of bugs may be eligible for a reduced bounty (non-comprehensive):

 - Backend service DoS bugs
 - Open redirect on any TurboWarp website
 - Scratch.canFetch(), Scratch.canOpenWindow(), etc. bypass in extensions in the [official extension gallery](https://github.com/TurboWarp/extensions) (including unlisted ones)

Guidelines:

 - Participation in this program is contigent upon you acting in good faith.
 - No bounties for bugs you created yourself.
 - The bug needs to work on the latest version on GitHub at the time of reporting.
 - The bounty can be sent in almost any form you desire or donated to a charity of your choice.
 - The decision about whether you get a bounty and the size is ultimately up to me.

Examples of bugs that might not be eligible for a bounty:

 - Bugs in upstream projects such as Scratch, Scratch Addons, Electron, Chromium, etc. Please report these to the appropriate upstreams.
 - Missing "security headers" such as X-Frame-Options or Content-Security-Policy without demonstrated impact.
 - Self-XSS.
