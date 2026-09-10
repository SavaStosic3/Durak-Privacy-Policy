---
title: Durak — Delete Your Account
permalink: /delete-account/
---

# Delete Your Durak Account

Last updated: 2026-09-10

Online accounts in Durak are optional — you only have one if you signed in to
play online. Offline play never requires an account.

## Delete in the app (fastest)

1. Open Durak and go to **Profile → Account**.
2. Sign in if you are not already signed in.
3. Tap **Delete account**, then confirm. If you signed in with Google or Apple,
   you may be asked to re-confirm with that provider — no password needed.

This permanently and immediately deletes your account and its data.

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

## What is retained

When you delete your account we remove your account record and the data you
created: your online stats and rating, your friends, friend requests, and
blocked-users list, and — unless your account was banned — your username and its
reservation. Three small things can remain, and a fourth if you were banned:

- **Rating records.** Each rated online match leaves one record of that match:
  its identifier, the accounts that took part, each player's rating before and
  after, the result, and the time. It holds no cards, deck order, or replay.
  These records are **automatically deleted one week after the match**, so at
  most a week's worth can outlive your account. They exist so a rating change
  can be explained or corrected, and they describe matches other players also
  took part in — which is why they expire on a fixed schedule rather than being
  erased when one participant leaves.
- **Safety records.** If you reported another player, that report is kept for
  safety and moderation — it is about them, not you — but **your identifier is
  removed from it** when you delete your account, so nothing links it back to
  you. Reports other players filed *about* you are deleted outright along with
  your account. All reports are in any case **automatically deleted 30 days
  after they are filed**.
- **A record that the deletion happened.** Your account identifier, the word
  "deleted", and the time — nothing else. Your sign-in credential stays valid
  for up to an hour after it is withdrawn, and this record is the only thing
  that tells our server the account behind it is gone; without it, a credential
  still in flight could bring the account back. It is **deleted automatically
  24 hours** after the deletion completes, by which time no such credential can
  still exist. If a deletion is interrupted part-way, this same record is what
  lets you resume it, and it is kept for up to 30 days so that you can.
- **A banned username.** If your account was banned for abuse before you deleted
  it, we keep the username itself, so that nobody can claim that name again. The
  record is the name and the date it was kept — nothing else. It holds no
  account identifier, no email, and no link back to you, it is never shown to
  anyone, and to other players the name simply reads as unclaimed and cannot be
  taken. This exists so a banned player cannot return under the same name, and
  so nobody else can take on a name other players have reason to remember. It is
  the only thing a deletion keeps indefinitely, and only after a ban.

Rating records and reports expire on a fixed schedule rather than when one
participant leaves: rating records one week after the match, reports 30 days
after they are filed. The record of the deletion goes 24 hours after it
finishes. A kept username lasts indefinitely, because a ban does.

If another player had blocked you, that block is removed when you delete your
account — once one side is gone it protects nobody.

## Can't open the app?

If you cannot sign in or open the app, email **support.durak@gmail.com** from the
email address on your account and ask us to delete your account. We will confirm
you control that address and then delete the account and its data.
