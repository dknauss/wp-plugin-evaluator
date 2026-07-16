# WordPress Plugin Evaluation Scorecard

A single-file, interactive tool for deciding whether a WordPress plugin — or a theme,
extension, or any other installable code — earns a place in a site you build, maintain,
or stake your name on.

**[▶ Open the live tool](https://dknauss.github.io/wp-plugin-evaluator/)** *(update this link once GitHub Pages is enabled)*

![Verdict: a weighted score and go/no-go recommendation](https://img.shields.io/badge/verdict-live%20scoring-2271b1)

## What it does

Work top to bottom through eleven numbered cards. As you go, a sticky bar keeps a live
weighted score, a percentage gauge, and a go/no-go verdict:

1. **Plugin Details & Classification** — metadata, plus whether the plugin is *Canonical*,
   *Commercial*, or *Community*, and where its source code lives (.org / GitHub / vendor / other).
2. **Fit Check** — the "right tool for the job" gate (Necessary? Functional? Compatible? Better than the alternatives?).
3. **Instant-Reject Filters** — baseline hard stops; fail one and the verdict is REJECT no matter the score.
4. **Maintenance & Longevity** — including a heavily-weighted check for **admin auto-updates**.
5. **Developer & Vendor Trust** — reputation, provenance, host bans, rug-pull risk.
6. **Support & Docs**.
7. **Hands-On** — function, performance (Query Monitor), conflicts, clean uninstall.
8. **UI/UX Tidiness & Ethics** — admin-notice behavior (the [dismissed.fyi](https://dismissed.fyi/) rubric), telemetry, dark patterns, accessibility.
9. **Licensing & Business Model**.
10. **Hard-Fail Overrides** — "passed the math, still a no."
11. **Decision** — record conditions, reasoning, review date, and owner.

Each signal is scored **0–3** (or **N/A**, which excludes it from the math, so the percentage
always reflects only what you actually rated). Section weights and the ×5 auto-updates weight
are applied automatically.

### Verdict bands

| Score | Verdict |
|------:|---------|
| ≥ 80% | Adopt |
| 65–79% | Adopt with conditions |
| 50–64% | Last resort only |
| < 50% | Reject |
| any | **Reject** if an instant-reject filter or a hard-fail override is triggered |

## Using it

- **No install, no build, no dependencies.** It's one self-contained HTML file — open it in any browser.
- **Nothing is saved.** Fill it out, then **Print / PDF**, **Copy Summary**, or **Download Report**
  (a filled-in Markdown file named per plugin) to keep a record.
- Runs entirely client-side. No tracking, no network calls.

## Credits

Built from three talks on choosing plugins wisely:

- Dan Knauss — *Effective Strategies for Picking WordPress Plugins* (WP YEG, 2025)
- Kathy Zant — *Evaluating Plugins: Strategies to Effectively Extend WordPress*
- Remkus de Vries — *How To Tell if a WordPress Plugin Can Be Trusted*

The admin-notice ethics rubric draws on Anchor Hosting's *Hall of Shame* and the
[dismissed.fyi](https://dismissed.fyi/) database, plus WordPress.org plugin
[Guideline 11](https://developer.wordpress.org/plugins/wordpress-org/detailed-plugin-guidelines/).

A companion prose field guide accompanies this tool for teams who want the full rationale.

## License

GPL-2.0-or-later. SPDX-License-Identifier: `GPL-2.0-or-later`. See [LICENSE](LICENSE).

Copyright (C) 2026 Dan Knauss.
