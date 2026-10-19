# Lostie Locator: Decisions log

Append one entry per decision so later work does not reopen it.
Newest at the bottom.

| Date | Decision | Why |
|------|----------|-----|
| 2026-10-12 | Project docs live in `docs/`, indexed from `CLAUDE.md`. | Every Claude session loads `CLAUDE.md`, so the docs are always found. |
| 2026-10-12 | Initial market is Belarus. | Where the team is based. |
| 2026-10-12 | Web app first, usable on laptop and phone browsers. | One codebase reaches every device. |
| 2026-10-12 | Private in-app chat; personal info shared only with both sides' approval. | Privacy and safety. |
| 2026-10-12 | English first, Russian localization next. | Faster start; Russian is the key follow-up. |
| 2026-10-12 | Moderation against spam, scams and fake found reports is required. | Trust in the reports. |
| 2026-10-12 | Found cases are closed and archived, not deleted. | Reunion stories help others and promote the app. |
| 2026-10-12 | All changes go through PRs; nothing is pushed without Dima's confirmation. | Dima reviews everything first. |
| 2026-10-13 | Nearby radius is user-configurable from 2 to 15 km. | Different areas (city vs countryside) need different ranges. |
| 2026-10-13 | Notifications: nearby feed, plus optional push when a report is created nearby. No email alerts. | Keep it simple; users opt in to push. |
| 2026-10-13 | An account is required to post or help. | Accountability and moderation. |
| 2026-10-13 | Moderation plan in `docs/moderation.md`: report button, review queue, new-account limits, automatic checks, chat scam warnings. | Dima approved the suggested plan. |
| 2026-10-13 | Default nearby radius is 5 km (still adjustable from 2 to 15 km). | Dima picked it as the starting value; users can widen it outside cities. |
| 2026-10-14 | Visual style: minimal and friendly ("style D"): white background, Onest font, warm coral accent (#D9480F), soft pastel Lost/Found labels, large rounded photo cards. | Dima preferred it over plainer and bolder options; Onest also covers Russian. |
| 2026-10-14 | Logo: "Searching paw", a magnifying glass with a paw print in the lens, in coral (#D9480F), next to the lowercase wordmark "lostie" in Onest. | Dima picked it from ten paw-based options. |
