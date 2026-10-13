# Roam Tour

**Roam Tour** is a gamified social travel platform that encourages people to explore real-world destinations through location-based quests, achievements, and community participation. It also gives local businesses a way to attract visitors by creating promotional quests and rewarding verified participation.

**Tagline:** Turn every trip into a game.

## Overview

Roam Tour connects two primary audiences:

- **Travelers** discover destinations, participate in quests, track their progress, and share travel experiences.
- **Businesses** publish location-based quests, manage campaigns, and view basic engagement results.

The platform consists of a **mobile application for travelers** and a **web portal for businesses**, supported by a shared backend.

## MVP Goals

The minimum viable product (MVP) aims to validate whether travelers enjoy completing real-world quests and whether businesses find value in creating those quests.

The initial release focuses on a straightforward experience: travelers find a quest, visit a participating location, verify completion, and earn points. Businesses can create and manage quests without needing a complex advertising platform.

## MVP Features

### 1. Traveler Mobile Application

#### Account and Profile

- Register and sign in using email and password.
- View a personal profile with accumulated points, earned badges, and completed quests.
- Update basic profile information.

#### Quest Discovery

- Browse available quests in a list.
- Discover quests on a map using location information.
- View quest details, including location, instructions, point rewards, and availability.
- Filter quests by category or nearby location.

#### Quest Participation and Verification

- Start an available quest.
- View quest requirements and completion status.
- Check in at the location and scan a quest-specific QR code to submit completion.
- Validate proximity to the location when location permission is granted.
- Prevent duplicate rewards for the same non-repeatable quest.

**MVP verification approach:** Use QR-code check-in with a location-proximity check for eligible quests. Verification requirements must be transparent to users, and suspicious or invalid submissions should not award points.

#### Points and Achievements

- Award points for verified quest completion.
- Track total points and quest completion history.
- Unlock a small initial set of badges based on defined milestones.

#### Leaderboard

- View a basic leaderboard ranked by earned points.
- Display the traveler's current rank when applicable.

#### Travel Activity Feed

- Create simple travel posts with a caption and optional photo.
- Browse recent posts from other travelers.
- View posts associated with completed quests or visited places.

The MVP feed is intentionally limited; advanced social networking features are reserved for later releases.

### 2. Business Web Portal

#### Business Accounts and Profiles

- Register or sign in as a business user.
- Create and maintain a business profile with name, description, and location.
- Submit a business for basic administrator review before publishing quests.

#### Quest Management

- Create quests associated with an approved business location.
- Set a quest title, description, instructions, category, point value, and availability dates.
- Publish, pause, and close quests.
- Generate and display QR codes for in-person quest verification.
- Review basic participation and completion counts.

#### Basic Dashboard

- See active and completed campaigns.
- Track quest participation and verified completions.
- Identify which quests receive the most engagement.

### 3. Platform Administration

A lightweight administrative interface or protected internal workflow will support the MVP by allowing authorized operators to:

- Review business registrations.
- Moderate or disable inappropriate quests and travel posts.
- Investigate flagged completion attempts.
- Configure initial quest categories, point rules, and badge criteria.

## Core User Journeys

### Traveler Journey

1. Create an account and complete a basic profile.
2. Discover a quest in the mobile app.
3. Review the requirements and visit the destination.
4. Scan the designated QR code and pass required verification checks.
5. Receive points after successful completion.
6. Track progress, view the leaderboard, and optionally share a travel post.

### Business Journey

1. Create a business account and submit business details.
2. Receive approval to publish quests.
3. Create a location-based quest and define its completion rules.
4. Display its QR code at the participating location.
5. Monitor completion counts and basic engagement metrics.
6. Update, pause, or close the quest as needed.

## MVP Quest Types

The first release will prioritize quest types that can be verified consistently.

| Quest type | Example | Verification |
| --- | --- | --- |
| Location visit | Visit a participating cafe | Location proximity and QR scan |
| Landmark exploration | Check in at a selected attraction | Location proximity and designated QR scan |
| Business promotion | Visit a partner store during a campaign | Business QR scan and applicable location check |

Purchase-dependent rewards, receipt analysis, multi-stop itineraries, and complex photo challenges are not required for the initial MVP.

## Platform Components

| Component | Primary users | Responsibility |
| --- | --- | --- |
| Traveler mobile app | Travelers | Discovery, quest completion, points, leaderboard, posts |
| Business web portal | Business operators | Business profiles, quests, campaigns, basic analytics |
| Administration | Platform operators | Reviews, moderation, configuration, fraud investigation |
| Backend services | All applications | Authentication, quests, verification, rewards, location data, posts |

## Key Product Rules

- Points are awarded only after server-side verification succeeds.
- Each quest has a defined availability period and completion policy.
- Non-repeatable quests cannot be completed multiple times by the same account.
- Business users may publish quests only for approved business locations.
- QR codes must be validated on the server; scanning a code alone must not guarantee points.
- Location permission must be requested clearly and used only when relevant to quest verification or discovery.
- Moderation controls must exist for misleading quests and inappropriate public content.

## Out of Scope for the MVP

The following capabilities are potential future enhancements, not commitments for the first release:

- Paid advertising subscriptions and automated business billing.
- Redeemable points, vouchers, and financial rewards.
- Global, country, city, seasonal, and friends-only leaderboard variations.
- Direct messaging, follows, comments, and complex social interactions.
- AI-powered quest recommendations.
- Multi-location quest chains and personalized itineraries.
- Receipt recognition, automated photo verification, and advanced anti-fraud scoring.
- Offline quest completion and international localization.

## MVP Success Metrics

Roam Tour will evaluate early adoption using a small number of measurable indicators:

- **Traveler activation:** Percentage of registered travelers who complete at least one quest.
- **Quest completion rate:** Percentage of started quests that are successfully completed.
- **Repeat engagement:** Percentage of active travelers who complete another quest within 30 days.
- **Business activation:** Percentage of approved businesses that publish at least one quest.
- **Campaign engagement:** Verified completions per published quest.

These measures help determine whether to expand the quest system, social features, or business monetization.

## Project Status

**Stage:** MVP planning and development.

Features documented here represent the intended MVP scope and should not be interpreted as already implemented.

## Product Vision

Roam Tour aims to make local exploration more engaging while helping businesses connect with travelers through meaningful real-world experiences. The MVP establishes the foundation: discover places, complete verified quests, earn recognition, and measure participation.
