# LonelySky public journey totals

Public aggregate statistics for [LonelySky](https://lonelysky.app/). This repository contains only this notice, `.nojekyll`, and `public-stats/journey.json`.

The private game repository reads a fixed Google Analytics report and updates this snapshot every three hours. GitHub Pages serves the JSON; the game's CDN caches it. This repository has no application code, credentials, individual journeys, coordinates, messages, or player identifiers.

`travelers` counts GA4 browser users who reached `game_ready` over the stated reporting period. It is not a count of natural persons or people currently online. `launches` and the interaction totals are event occurrences, not unique people. Letter confirmations can include recovery of an accepted letter; coflight connections can be reported by each participating client.

Flight time is active, unobstructed in-game flight time; distance uses game units, not light-years. Missing historical events remain `null` (unknown). Zero and unknown are different. Reports end on the previous day in the property's time zone, and analytics processing can lag. The game may display explicitly labeled local estimates between snapshots, capped at 24 hours; the JSON itself contains measured aggregates only.

Schema version: `1`. An `unavailable` status means the latest report could not be safely read; it must not be presented as a successful zero-value report.
