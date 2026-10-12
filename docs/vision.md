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

## Open questions

These are not decided yet; answers go into `requirements.md`, `tech.md` or
`decisions.md`.

- Platform: mobile app, web app, or both? Which first?
- How "nearby" is defined (radius, city, district) and how helpers get notified.
- How owners and finders/helpers contact each other, and how much personal
  data (phone, exact address) is shown publicly.
- Languages for launch (Russian, Belarusian, English?).
- Moderation: preventing spam, scams and fake "found" reports.
- Does a case get closed/archived when the pet is found?
