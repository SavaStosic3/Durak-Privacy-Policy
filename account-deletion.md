---
title: Durak — Delete Your Account
permalink: /delete-account/
---

# Delete Your Durak Account

Last updated: 2026-09-17

Online accounts in Durak are optional — you only have one if you signed in to
play online. Offline play never requires an account.

## Delete in the app (fastest)

1. Open Durak and go to **Profile → Online account**. If the age/Terms screen appears,
   choose **Delete an existing account** to use your current signed-in session
   without accepting updated Terms.
2. If you are signed out, use the email option below, or return to the regular
   account screen to sign in.
3. Tap **Delete account**, then confirm. If you signed in with Google or Apple,
   you may be asked to re-confirm with that provider — no password needed.

When the app confirms success, the active sign-in account and the primary
Durak account data listed below have been deleted. This cannot be undone in the
app. If deletion is interrupted or an error appears, retry or contact support;
starting the request does not mean every step has finished. Account closure
does not erase every operational record or provider copy immediately.

## What is deleted

- Your account and sign-in credentials (email and password), held by Firebase
  Authentication.
- Your public username and its reservation. (If your account was banned for
  abuse, the name itself is kept so it cannot be claimed again — see below.)
- Your online stats (games played, wins, losses, and streaks).
- Your online rating (Elo) and your rated-game count.
- Your friends list, friend requests, and your blocked-users list.

Offline data on your device (offline stats, achievements, saved games, and
cosmetics) is stored only on your device and is removed when you delete the app.

Deleting your account does not cancel or refund a cosmetic pack you bought.
Purchases belong to your App Store or Google Play account, not your Durak
account, so after a reinstall you can restore them with **Restore Purchases**
on the same store account — on the same platform you bought them on.

## What is retained

Some records have a different purpose and deletion process:

- **Rating and integrity records.** Shared match records retain match and
  participant identifiers, rating changes, outcome and timing for disputes and
  result verification. Failed rating-update records support investigation.
  They become eligible for automatic deletion seven days after the server
  writes them, which can be later than the match. Rewriting a failed-update
  record restarts its expiry. They contain no cards, deck order or replay.
  Duplicate-credit markers also have a seven-day expiry from writing and are
  removed with the account during successful account-data deletion.
- **Safety records.** Reports you filed about others have your reporter
  identifier replaced during successful account-data deletion. Reports matched
  to your account as their subject are removed. A report about an unresolved
  username may not be matched to an account; it follows the report expiry
  instead. All reports become eligible for automatic deletion 30 days after
  filing, whether reviewed or not. Removing a reporter identifier does not
  guarantee anonymity: moderation notes can still identify people.
- **Deletion records.** An account identifier, deletion state and timestamps
  help block access and resume interrupted requests. A completed-deletion
  record receives an expiry 24 hours after completion is recorded. A pending
  record receives an expiry 30 days after the latest deletion attempt; another
  attempt resets that pending expiry. Expiring this record does not complete a
  failed deletion or erase remaining account data.
- **A banned username.** Its reservation keeps the username, ban-reservation
  status and date, without the account identifier or email, to prevent reuse
  and impersonation. The username can still identify its former owner. There
  is no automatic expiry; the developer reviews reservations at least
  quarterly and on correction requests, and removes those no longer necessary
  or created in error. Other players cannot open a profile for the reserved
  name, and it cannot be claimed.
- **Room and matchmaking records.** Room state, directory entries and
  active-match reservations have a separate server-cleanup lifecycle. They can
  contain account or guest identifiers while cleanup is outstanding, and are
  not covered by an immediate account-deletion deadline.

These expiry times make records eligible for managed database cleanup. Physical
deletion happens asynchronously and can be delayed; the times are not guarantees
that every copy is gone. Cloudflare logs, authentication-provider records,
support correspondence and recovery copies follow separate retention processes
described in the [Privacy Policy](https://savastosic3.github.io/Durak-Privacy-Policy/).
Restored account data must be reconciled with subsequent deletion requests and
expired records before returning to service.

If another player had blocked you, that block is removed during successful
account-data deletion.

## Can't open the app?

If you cannot sign in or open the app, email **support.durak@gmail.com** from the
email address on your account and ask us to delete your account. We will confirm
you control that address and then delete the account and its data.
