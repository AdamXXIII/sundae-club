# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Delegated: Adam left the choice to Claude. Existing site is a single static `index.html` with inline CSS and media in `media/`, hosted on GitHub Pages. Keep it static (no build step) unless a real need appears.

## Users

Players: people deciding whether to download a free Windows playtest of an online co-op horror game. Likely friends and friends-of-friends of Adam, plus co-op/horror gamers who find the link. They need to understand the game in under a minute, trust the download, and know how to get a crew together.

## Product Purpose

The website for Sundae Club, Adam's Godot co-op game. It exists to get visitors to download the installer and play with friends. Success is downloads (counted via GitHub release download counts) and crews starting a first co-op night.

## Positioning

Online co-op horror for 1 to 8 players (best with 4) where you paint your suit the colour of the walls to hide from monsters and film them for views. Camouflage-as-defence plus the content-creator crew framing (an ice cream van by day, a horror channel by night) is the hook no other co-op horror game truthfully shares.

## Operating Context

- Public repo `AdamXXIII/sundae-club` holds the site and installer releases only; game code stays private.
- Site: https://adamxxiii.github.io/sundae-club/ (local copy at `D:\sundae-club-site`).
- Download button points at `releases/latest/download/SundaeClub-Setup.exe`, so shipping a release (`tools/release.ps1 <version> "notes"` in the game repo) updates the site automatically.
- Current build: Playtest v0.2.0, Windows 10/11, 147 MB, free. Windows may warn on install (More info, then Run anyway).
- Game is in polish-only mode (no new features since 2026-10-17). Steam is a possible later step if the playtest goes well.

## Capabilities and Constraints

- Windows only. Co-op networking over UPnP is untested between two PCs as of the last note; do not promise easy online play beyond what is verified.
- Game facts the site may state: pure co-op (no traitor), 60 seconds to hide/paint/run when the alarm goes, no on-screen monster warnings (3D sound only), the depot is a safe zone, sponsors are shout-outs with a monster in the background.
- Static hosting only; no accounts, backend or analytics unless Adam chooses to add them.

## Brand Commitments

Name is "Sundae Club". Voice is dry, playful and second-person ("Paint yourself in. Film the monsters. Go viral or go missing."). The existing site already commits to a night-shift van-crew world with a camcorder (REC dot and timestamp) framing for screenshots; treat that as incumbent, not as a binding spec for new work.

## Evidence on Hand

Real in-game screenshots, crew portraits (Rexx, Rocky, Rookie, Thena), monster art, fake sponsor ad videos (Brave Bean, Crumbs, Gloop, Vanguard) and a hero video, all in `D:\sundae-club-site\media\` and `D:\Sundae Club\promo\`. No reviews, press, player counts or testimonials exist; never fabricate them.

## Product Principles

1. Show the game before explaining it: real footage and screenshots lead.
2. Honest about being a free, early playtest; no inflated claims.
3. One obvious action: download, with install steps and the Windows warning explained up front.
4. Make it easy to bring friends; it is a co-op game.
5. Humour comes from the game's world, never from graphics-only gimmicks.

## Accessibility & Inclusion

Adam has not set a required standard. Respect reduced-motion (the site already does), keep text readable on a dark theme and make it work on phones, since friends often open links there.
