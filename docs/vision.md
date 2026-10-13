# Lostie Locator: Vision

## The problem

People lose their pets. When a dog or cat goes missing, the owner's best chance
of getting it back is the people nearby: neighbours, passers-by, anyone who
might have seen the animal. Today there is no simple, dedicated place to reach
those people quickly with a photo, a description and a last-known location.

The reverse also happens: someone finds a pet that looks lost and has no easy
way to tell the owner "I think I have your pet."

## What Lostie Locator is

An application that connects people who **lost** a pet with people **nearby**
who can help find it, and people who **found** a pet with the owner who is
looking for it.

## Core ideas

1. **Lost pet request.** An owner posts "I lost my pet, I need help" with a
   photo, a description and where/when it was last seen.
2. **Help from people nearby.** People close to that area see the request, look
   at the photo and description, and can help: mark the location where they
   saw the pet and add any information related to the case.
3. **Found pet report.** Someone who finds a pet that looks lost posts a page
   saying "Looks like someone lost this pet, are you looking for it?"
4. Lost and found reports for the same animal should be easy to connect so the
   pet gets home.

## Who it is for

- **Owners** who have lost a pet.
- **Helpers**: people nearby willing to keep an eye out and report sightings.
- **Finders**: people who have found a pet that looks lost.

## Where we start

The initial market is **Belarus**, with the long-term aim of being useful to
people anywhere in the world.

## What success looks like

More lost pets get back to their owners, faster.

## Key product decisions

See `decisions.md` for the full log.

- **Platform:** a web app first, usable from both laptops and phone browsers.
- **Nearby:** the owner shares whatever last location they have. Reports are
  shown in a feed of recent posts near each user. The radius is configurable by
  the user from 2 to 15 km.
- **Notifications:** the nearby feed, plus optional push notifications when a
  new report is created nearby.
- **Accounts:** posting a report or helping on one requires an account.
- **Contact:** owners, finders and helpers talk through private in-app chat.
  Personal information is never shared without the approval of both sides.
- **Language:** English first; Russian localization comes next.
- **Moderation:** required, to prevent spam, scams and fake "found" reports.
- **Closed cases:** when a pet is found, the case is closed and archived, not
  deleted. Reunion stories stay visible as a reminder to others and to promote
  the app.

## Open questions

- How moderation works (user reports, manual review, automatic checks).
- Default radius within the 2–15 km range.
