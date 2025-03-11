+++
title = "Elite: Dangerous on Steam Deck"
date = 2025-03-11
+++

## Background

I recently got back into playing Elite: Dangerous after a several year hiatus, primarily due to excitement around a potential Distant World 3 in 2026. The last time I really played was around Distant Worlds 2 in 2019, turns out spending literal months doing nothing but jumping to the edge of the galaxy and back takes it out of you. Despite that, I for some reason want to do it again!

Anyway, another reason I stopped playing is because I have moved a lot of my gaming over to the Steam Deck. The deck runs Elite surprisingly well, even with graphics set to medium, especially if all you're doing is flying instead of doing a lot of exploration on planets. But Elite is one of those games where you often have other applications and sites open, like EDSM and Inara, and for that you really want to have the Elite Dangerous Market Connector running to automatically track your progress. When the deck first came out there wasn't an easy way to run EDMC alongside Elite and that made it not worthwhile to play long term if my progression wasn't being tracked correctly.

## EDMC on Deck

It's 2025 now and both the Steam Deck itself has more capabilities and more software is being built for (or at least with) the Steam Deck in mind. Most notably, you can now run two or more applications at once while in `game` mode on the deck, and there's a version of EDMC that is designed specifically for installing on steam decks.

### Installation Guide

There are likely other tutorials out there, but there were parts of the install that weren't obvious to me and that caused me some troubles, so here's my notes on installing it.

1. If you haven't yet, start Elite: Dangerous and load up a ship. Once it's loaded you can exit the game. We want to make sure the journal files exist.
2. We'll do the first part of the install in `desktop` mode, but you don't need a mouse and keyboard if you're comfortable with using the trackpad and onscreen keyboard. Start by loading into the desktop.
3. The [EDMC version](https://github.com/flathub/io.edcd.EDMarketConnector) being installed is a flatpak but I could not find it in the store, so we will install it manually.
4. From the start menu, open a new terminal by searching for `terminal` or finding the `konsole` application. I recommend moving it to the top half of the screen so the keyboard doesn't block it.
5. Open the on-screen keyboard (steam key + x button) and type the following to install the flatpak.  It may be easier to open this page in the web browser on the deck so you can copy and paste this and several other strings.

```bash
flatpak install flathub io.edcd.EDMarketConnector
```

6. Once installed, it should be in the `games` folder in the start menu, next to `Elite Dangerous`. Find it, right click, and click "Add to Steam" so we can launch it later in game mode.
7. While still in desktop mode, open EDMC. It is easier to do the configuration now, before using it later in game mode.
8. You will need to authenticate with Frontier, I believe it popped up a browser automatically for me but it might have been after the step below.
9. If it doesn't automatically fill, we need to populate the journal folder in the settings. Per the github repo, that folder should be the following. Note that right click and paste doesn't seem to work, but if you open the on-screen keyboard there's a paste option that does work.

```bash
~/.steam/steam/steamapps/compatdata/359320/pfx/drive_c/users/steamuser/Saved Games/Frontier Developments/Elite Dangerous
```

10. Next, populate the EDSM, Inara, and other API keys depending on which services you want to upload data to. This is the same as on a normal desktop, but keep in mind that pasting only works through the on-screen keyboard.
11. At this point it should be fully functional. I recommend testing in desktop mode at least once by launching Elite. You can run it in windowed mode at a low resolution so you can easily see both windows and just make sure it's reading your journal files correctly.

#### Using in Game Mode

Assuming you've got it working in desktop mode, you don't want to always have to be in desktop mode just for this one game. Here's how to use it in game mode.

1. If you didn't already, make sure while in desktop mode to right click the EDMC in the start menu and select "Add to Steam" so we can launch it in game mode.
2. In game mode, go into the library. You should find `E:D Market Connector` in the list of installed "games". Start it.
3. It should start as just a small window in the middle of a large border of black. It ain't pretty, but you should still be able to interact with it like normal.
4. Press the steam button, then launch Elite Dangerous either through the Library or Home menus.
5. Now when you press the steam button, you should see both EDMC and Elite running at the same time.
6. Log into Elite, load up a ship, and try flying to another system or re-docking at your current one. When you swap to EDMC through the steam menu it should be updating as expected.
7. When you're done playing Elite and quit to desktop, make sure to also close the EDMC window.

## Conclusions

Hopefully that answers some questions about how to get EDMC running on the steam deck in game mode. That was the biggest hurdle for me to play on deck and now that it's easy to run both applications at once I'm much more interested in picking up the game and doing a few exploratory or trading hops without having to fire up my whole desktop. My interests shift a lot, so I might not keep up with it all the way until Distant Worlds 3 starts, but I'd like to get my Trading rank up to Elite since I've been sitting at Tycoon for literally years at this point. I haven't done much of the first-person stuff that was added with Odyssey, so maybe I'll try my hand at some of that too. Anyways, fly safe Commander! o7
