# Funding: Free, Ad-Free, and Transparent

This document explains how the app pays for itself without subscriptions, paid tiers, or ads. It puts [VALUES.md](VALUES.md) principle 11 into practice.

**Status:** this is the intent. It gets built in Phase 7 of the [roadmap](ROADMAP.md), after the friends-and-family test. Nothing here is needed before then, but it is written down now so earlier decisions (especially backend costs in session 4.2) keep it in mind.

## Why

Many self-help and planning apps lock their most useful features behind a subscription or fill the app with ads. That shuts out a large group of people who need the help most, and ads compete for the attention the app is trying to protect. This app takes a different path: everyone gets the whole app, free, and anyone who wants to can help keep it running.

The trade-off is accepted on purpose. Without subscriptions or in-app sales, the app earns less, and the app stores may promote it less. That is fine.

## How it works

1. **A yearly goal.** The app shows how much it costs to keep it available for one year.
2. **A cost breakdown.** The goal is split into its parts, so people can see exactly where their money goes.
3. **A progress bar.** It shows how much has been donated toward this year's goal.
4. **How people can help.** A short, calm explanation of how to donate, and that sharing the app with a friend also helps.
5. **When the goal is met.** The page says so, thanks everyone, and explains clearly that anything donated beyond the goal goes to the app's developers, with real appreciation.

## Where it lives in the app

- A "Support the app" page, reachable from settings or an "About" screen.
- It never interrupts planning, never pops up uninvited, and never blocks a feature.
- At most, a gentle mention in a natural place, such as the Sunday week report once a year. The exact rule is decided in design, and it must pass the values check: no guilt, no false urgency.

## Costs to include in the breakdown

These are the known or likely costs. Confirm the real numbers in sessions 4.2 and 7.1, because prices change.

| Cost | Rough amount | Notes |
| --- | --- | --- |
| Apple Developer Program | $99 per year | Needed to publish on the App Store |
| Google Play developer account | $25 one-time | Could be spread over the first year's goal |
| Backend for sign-in and encrypted backup | Depends on 4.2 | Many services have a free tier at small scale, so this may start at $0 |
| Build service (Expo EAS) | $0 on the free plan | Only becomes a cost if the free build limits are not enough |
| Store fees on donations | A percentage of each donation | See the open questions below |
| Domain and privacy policy hosting | Small, optional | A privacy policy URL is required by both stores |

## Open questions (to check in session 7.2)

These are not decided. They are real constraints to research before building the page.

- **App store payment rules.** Apple and Google both have rules about collecting money inside an app. In general, tips or donations to a developer (not a registered charity) may have to go through their in-app purchase systems, which take a percentage. Registered nonprofits can sometimes use other options. These rules have been changing, especially in the US, so check the current guidelines rather than relying on this note.
- **Where the progress number comes from.** The app needs a trustworthy source for the "donated so far" amount. It could be a manual number you update, or one read from the payment provider. Simple and honest beats clever.
- **The word "donation".** In many places "donation" suggests a registered charity and tax deductibility. Since money goes to an individual developer, wording such as "support" or "tip" may be more accurate. Check this, and say plainly in the app that it is not tax-deductible if that is the case.
- **Taxes.** Income from donations or tips is usually taxable for the developer. Worth a quick check before launch.
