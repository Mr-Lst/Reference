# Discord Nitro Boost Badge Persistence Vulnerability

## Overview
This document describes a logic vulnerability found in Discord's Nitro Boosting system that allows users to retain the "Server Booster" badge indefinitely, even after their Nitro subscription expires.

## Vulnerability Details
- **Product:** Discord (Web, Desktop, Mobile)
- **Affected Versions:** All versions as of July 2025
- **Component:** Nitro Boosting System, Badge Logic

## Description
Discord provides users with Nitro subscriptions that allow them to boost servers. When the Nitro subscription expires, a 3-day grace period is given. However, if another user boosts the same server during this grace period, the original booster’s badge is reactivated permanently, despite their subscription having ended.

## Impact
The vulnerability results in users retaining visual privileges (the Server Booster badge) they no longer qualify for, which can mislead other users and affect server dynamics.

## Steps to Reproduce
1. User A boosts a Discord server using an active Nitro subscription.
2. User A's Nitro subscription expires, starting a 3-day grace period.
3. User B boosts the same server during this grace period.
4. User A's booster badge remains permanently active, even without an active Nitro subscription.

## Disclosure Timeline
- Vulnerability discovered: July 2025
- Reported to Discord: [Date you reported]
- Awaiting fix as of submission

## Contact
Discovered by: @mx.lst & @luca_idk_myname_ 
