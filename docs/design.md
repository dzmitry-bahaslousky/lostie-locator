# Lostie Locator: App design

The clickable wireframes live on a design canvas:
https://claude.ai/artifact/NaBqDQwDWzReB2Cm5P24Ep (private; ask Dima for access).
This doc is the written summary. Where they differ, the canvas wins for layout
and this doc wins for behaviour.

## Look and feel

Minimal but friendly ("style D", chosen 2026-10-14).

- **Background:** white `#FFFFFF`; soft surfaces `#F6F4F1`, photo placeholders `#EFECE7`.
- **Text:** ink `#22201C`, secondary `#6B665E`. Borders `#EEEAE4`.
- **Accent:** warm coral `#D9480F` for the main action on each screen (Post,
  Continue, Send sighting) and for the logo.
- **Lost / Found labels:** soft pastel pills. Lost: `#FDEBDD` background,
  `#A63A0A` text. Found: `#E3EDFC` background, `#1E4FA8` text.
- **Home again:** green `#2F5D2A` for reunion stories and the Close case button.
- **Type:** Onest (Google Fonts; covers Cyrillic for the Russian version).
- **Shapes:** generously rounded: cards and photos 20px, inputs 16px, main
  buttons fully rounded pills. Touch targets at least 44px.
- **Tone of copy:** warm and plain ("3 pets need help near you",
  "Is this your cat?"), never alarming.

## Logo

"Searching paw" (chosen 2026-10-14): an outlined magnifying glass with a paw
print in the lens, in coral, next to the lowercase wordmark **lostie** in Onest
bold. On coral backgrounds (app icon) the mark is white. It is drawn on a
64×64 grid:

```svg
<svg viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
  <circle cx="27" cy="27" r="17" fill="none" stroke="#D9480F" stroke-width="6"/>
  <path d="M40 40L54 54" stroke="#D9480F" stroke-width="8" stroke-linecap="round"/>
  <ellipse cx="27" cy="31" rx="5.6" ry="4.6" fill="#D9480F"/>
  <circle cx="19.8" cy="24.5" r="2.4" fill="#D9480F"/>
  <circle cx="24.3" cy="20.3" r="2.4" fill="#D9480F"/>
  <circle cx="29.7" cy="20.3" r="2.4" fill="#D9480F"/>
  <circle cx="34.2" cy="24.5" r="2.4" fill="#D9480F"/>
</svg>
```

## Navigation

Phone: a bottom bar with **Nearby** (feed), a coral **Post** button, **Chats**
and **Profile**. Laptop: the same items in a top bar, with the feed list next
to a map.

## Screens

1. **Nearby feed.** Headline with the count of pets needing help, the user's
   area and radius (tap to change), filter pills All / Lost / Found, and big
   photo cards (label, distance, time, short description). Reunion stories
   appear in the feed as "Home again" cards. A list/map toggle is planned.
2. **Report detail.** Photo gallery, name, animal and breed, how to approach
   the pet, last seen time and place. A map shows the last-seen spot and every
   sighting; the sightings list sits below. Actions: **I saw this pet** and
   **Message owner**. Share and report (flag) in the header.
3. **Add a sighting.** Drop a pin on the map (or use current location), pick
   when (just now / within an hour / earlier), say how sure you are (sure /
   maybe), add a note and an optional photo. The owner is notified.
4. **Private chat.** Linked to a report. A permanent warning never to pay
   before seeing the pet. Phone numbers are swapped only when both people
   accept a share request. Block and report from the menu.
5. **Post, step 1: lost or found.** Two large choices. Shows the new-account
   posting limit and the no-phone-numbers-or-links rule.
6. **Post, step 2: photos and details.** Up to 5 photos, animal type
   (dog / cat / other), name, breed and colour, how to recognise and approach.
7. **Post, step 3: where and when.** Pin on a map, date and time, and an
   option to show an approximate area (about 300 m) instead of the exact spot,
   e.g. when the pet went missing from home. Explains who will see the post.
8. **Close the case.** Was the pet found with help from Lostie, came home on
   its own, or closing for another reason. Thank helpers (they get a
   notification) and optionally share a reunion story and photo. The report
   is archived, not deleted.
9. **Profile.** Verification badge, tabs for My reports (with Edit and
   "Pet is home"), My sightings, and Closed cases.
10. **Settings.** Home area, radius slider 2 to 15 km (default 5 km) with a map
    preview, push alerts for new lost and new found pets nearby, language
    (English now, Russian soon), account, blocked people, sign out.
11. **Laptop feed.** Feed list on the left, map of nearby reports with the
    radius circle on the right.
12. **Landing page.** "Lost a pet? The people nearby can help you find it."
    with "I lost my pet" and "I found a pet" buttons, How it works (3 steps),
    a Found-a-pet section, Safe by design (private chat, verified accounts,
    no pay-to-return scams), Home again stories, and a sign-up for helpers.

## Ideas added during design

Not in the original requirements; kept because Dima did not object. Revisit if
they complicate the MVP.

- "Show an approximate area" when posting, to protect owners' home addresses.
- "Sure / maybe" on sightings, so owners can weigh them.
