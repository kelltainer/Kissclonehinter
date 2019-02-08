KissCloneHunter 3.2 for Diablo II LoD v1.14d
-Contact portal@portaldeamon.com for questions/issues about versions 1.4 and up
-You can also contact me on irc. I am PortalDeamon000 on irc.dcloneirc.net
-Original programmer -> (c) 2006 Fuhrmanator (Fuhrmanator@gmail.com)
-Based originally on CloneHunter 2.2 Created by Snarg
 
==========================================================
KCH Advanced:
	Designed to work with multiple minimized Diablo II windows, including sandboxed ones.
	
	System Requirements:
	 Can NOT be run in multiple user accounts
	 Must be run with administrator privledges
	 Windows 2000, Xp, Vista, Windows 7 (should work on others, but will not run on Win9x/ME)
	 Works on both 32 bit and 64 bit systems
	 Compatible with Sandboxie (run outside the sandbox)
	 ClearScreen hotkey in D2 must be the default 'Space' for the alternate exit to work properly
	 Hotkeys for vocalizations must be the default Numpad 0-7 for anti-idle to work properly
	 Standard 96 DPI (text size) otherwise some GUIs might display incorrectly

	Incompatible Software:
	 Redvex (will cause game to see the redvex ip instead)

	Controls:
	 KCH will ask for your settings on the first tab. These settings can be written into profiles in the ini;
		Just put them with the same syntax under a new section. Settings will be saved to the profile when you
		launch an instance with those settings
	 Pause will pause the window in the midst of hunting (but will not anti-idle)
	 Join Game will tell one window to join a specified game and hold it. Format is Game/Pass or Game//Pass
	 Leave Game will leave the game you are holding and continue hunting
	 Unload will stop hunting/holding that instance
	 Change Ip will change the hunted ip
	 Change Duration will change the delay between games
	 Copy Game/Pass will copy the selected Game/pass into the clipboard. If multiple windows are selected,
		a return character will be entered between each game//pass
	 
	Saved Settings/Profiles
	 If you are using sandboxie with kch advanced and you did not install sandboxie in the default location you can change it
		in the KCHadv.ini under Reserved, Sandboxie.
	 Profiles are saved automatically under the selected profile. To make more profiles, just make new sections in the KCHadv.ini
	 Note: For the game prefix to be random, set it to: (random), For the password to be the game number, set it to (default)
	 
	Requirements for Multiple Windows:
	 All windows will automatically be detected on launch. Unique window names are NOT required.
	 Sandboxie is fully compatible with KCH advanced. By default no modifications should be necessary.
	 Each window must have either a random or unique game prefix; If multiple windows are launched with the same prefix, they will create slightly different prefixes.
	 KCH Advanced will run an invisible client process (KCH2.4Client.exe) for each hunting/held window
	 !!!NOTICE!!! If KCH crashes or is closed unexpectedly it will be necessary to close the KCH2.5Client.exe
		processes manually using the task manager.

==========================================================
KCH Standard/Basic:
	System Requirements:
	 Must be run with administrator privledges
	 Windows 2000, Xp, Vista, Windows 7 (should work on others, but will not run on Win9x/ME)
	 Works on both 32 bit and 64 bit systems
	 ClearScreen hotkey in D2 must be 'Space' for the alternate exit to work properly
	 Hotkeys for vocalizations must be the default Numpad 0-7 for anti-idle to work properly
	 Standard 96 DPI (text size) otherwise some GUIs might display incorrectly

	Incompatible Software:
	 Redvex (will cause game to see the redvex ip instead)
	 Any Program that will change the window title while it is running
	 (If you are running reporter, turn off the 'Show Ip in Title' option)

	Controls:
	 KCH will ask for your settings on startup
	 Pause will pause the window in the midst of hunting
	 Hold Game will hold the game you are currently in (if say you joined a game manually)
	 Abandon Game will leave the game you are holding and continue hunting
	 Change Ip will change the hunted ips
	 Change Duration will change the delay between games
	 Default values can be changed in the KCHadv.ini
	 
	Requirements for Multiple Windows:
	 All windows must have a unique window name. (you can run the "Rename Windows" option if you need to)
	 All windows MUST be run with the minimized option "Run D2 Minimized"
	 For Sandboxie run KCH inside each sandbox.
	 A new KCH must be run for each window.

==========================================================

Included Files:
 KissCloneHunter3.2.exe - Executable to run for KCH
 KCH3.2Client.exe - child process run by KCH advanced
 KCHReporter.exe - SOJ Sale Reporter program, will only run if specified. Due to security reasons, this file is not open source.
 KCHadv.ini - Saved Settings for KCH
 KCHlog.txt - Generated Log file
 readme.exe - this file
 tada.wav - sound file played on game found. Can be deleted or replaced
 dropped.mp3 - sound file played on game drop. Can be deleted or replaced
 Autoit source (folder) - contains source code of all recent versions

----
 
Technical notes:
 This program relys on memory reading, which will sometimes fail to work properly. The only known solution is to restart.
 KCH will run properly if the workstation is locked.
 KCH will run properly if the screensaver is active.
 KCH will run properly if user is logged in on another account.
 KCH will NOT work if the workstation is locked and requires Ctrl Alt Del to log in
 
----
 
Performance Tip:
 KCH may experience failures if the system is running at a very high cpu usage.
 To reduce the cpu usage of Diablo II you can wait until the window has joined its first game, then click inside the window,
 then select another window minimizing it. Usually this will reduce the cpu usage of Diablo II close to 0%. (it may take a few tries)
 
----
 
For the latest program (for Diablo 2 version 1.13d) visit http://www.portaldeamon.com/ or use the built in update feature.
Original Old Version -> http://pages.videotron.com/filmore/kch/

==========================================================
Changelogs:
Update 3.2 2016-6-09
-Updated for Diablo 2 1.14d

Update 3.1 2016-5-21
-Changed GameInfo Struct offset back to a pointer, as it was not working on some systems.
-Changed IPAddress offset to not use the gameinfo struct.

Update 3.0 2016-5-19
-Updated for Diablo 2 1.14c

Update 2.9 2016-3-19
-Updated for Diablo 2 1.14a
-Changed code compilation to not trigger anti-virus warnings
-Removed startup sound clip

Update 2.8 2013-6-27
-Fixed a serious bug that could cause KCH to become unresponsive when trying to launch many windows.

Update 2.7 2012-12-10
-Updated reporter system to use a dynamic ip address.

Update 2.6 2011-10-30
-Updated to work with Diablo II version 1.13d

Update 2.5 2011-9-26
-Altered Startup GUI to encourage more KCH "Advanced" use over "Standard"
-Fixed exception error when manually checking for updates under advanced
-Removed erroneous message boxes when renaming windows
-Altered compilation method to reduce size
-Removed KCH Standard option to not run minimized
-Removed broken KCH Standard option to notify an account on success
-Removed unnecessary KCH Standard function of doing warning beeps
-Removed useless tab send after game creation
-Reduced memory calls
-Added user permissions detection
-Added detection for incorrect sandboxie folder setting
-Removed the "Default" KCH Advanced settings profile
-Added the date to log entries
-Added Group field to KCH Advanced GUI
-Prevented KCH from sending soj reports for old counts/walks
-Fixed bug that prevented the Group setting from being saved to the ini
-Added link to the Soj Counts Webpage
-Added option to force groups to hold only 1 game per server
-Added sounds when sales/walks are detected
-Added option to hold a game from the KCH Advanced Startup Tab to quickly hold games
-Now removes displayed client information if the KCH Client errors
-Fixed issue that could cause kchreporter to not always report a sale

Update 2.4 2010-11-03
-Added Optional Soj Sale/Walk Reporter
-Added Sale/Walk detection for all Diablo 2 languages.
-Added KCH Advanced heavy logging ini override to log all games created
-Fixed GUI to not exit when Escape is pressed
-Fixed bug that simultanious triggering of a ftj and delay after X games caused a near infinite loop of waiting.
-Added support for Diablo 2 with resolution of 640x480
-Improved KCH Advanced error messages to include the window title
-Fixed KCH Advanced logging issue that could result in some messages not being logged
-Fixed KCH Advanced rare logging issue that could log the wrong ip

Update 2.3 2010-7-19

-Fixed create game function to work better with slow/failed creates
-Fixed exit game function to work better with slow/failed exits
-Changed the Join Game function to have all selected windows join the game (for muling or other purposes)
-Fixed the 'Wait' condition to allow affected windows to manually join a selected game
-Improved create game function error checking
-Improved rejoin game functions slightly
-Improved join game function slightly
-Fixed advanced change ip function to show the currently hunted ips by default
-Fixed bug that caused windows under the 'Wait' condition to not check for sales/walks
-Fixed bug that caused 'Rename Windows' to not properly rename more than 2 sandboxed windows

Update 2.2 2010-3-24

-Updated to work with Diablo 2 version 1.13c

Update 2.1, 2010-2-11

-Updated to Autoit 3 version 3.3.2.0
-Fixed broken Soj Sold/Walk Detection, with adv kch addition
-Reworked KCH Advanced Launch so multiple windows can be started with the same prefix setting
-Added .ini option to change the DelayBeforeNewGame setting (default is 5 seconds)
-Added Standard KCH .ini options to change the default game settings for KCH Standard
-Improved Update function to avoid browser file cache issues
-Fixed spacing on Current Ip Address Field
-Added sandbox compatibility for the Rename Windows function
-Fixed Sandboxed advanced clients to save log files in the correct location
-Fixed to show correct game/pass at every game
-Added ability to pause or start joining a game while in the lobby
-Added option to auto check for updates at startup
-Added Groups for multiple advanced windows, will pause other windows in the group after 4 locks on the same ip
-Fixed invisible drop-down combo boxes for Windows 2000 users
-Added options to stop or wait for a specified time after X games or X minutes.
-Changed logging to show window names under advanced mode
-Improved several error checking protocols

Update v2.0, 2009-6-16

-Added Advanced KCH Multi-Window Option. (completely rewritten display and control methods)
	includes many new features for users hunting multiple windows
-Advanced version now supports controlling Sandboxed windows as if they were normal
-Added logging on game found/held/sales/dropped/rejoining
-Added dropped game sound file and feature
-changed the Rename Windows function to rename any duplicate d2 windows
-added ability to minimize KCH
-fixed bug when clicking 'Hold Game' after failing to create previous game
-fixed input box positioning
-fixed kch standard having the edit box stop updating after reaching 30,000 characters
-fixed minimized send and mouse functions to not exit the program on error
-disabled "Hold game on SoJ sale or Walk msg" option as it does not work for most systems.
-added ability to pause the game after failing to create previous game
-changed autoit options to only pause script if chosen from the icon right click, instead of when clicking on the icon
-renamed the 'Run Minimized' to 'Run D2 Minimized' so it is clearer
-change exitgame function to not send {Space} beforehand
-improved update function for more dynamic updates in the future

----

Update v1.9, 2009-2-25

-fixed major bug involving ControlSend resulting in the keyboard having shift/alt/control gettting stuck down
-fixed failure to exit the first game properly issue.
-fixed bug in logging; now puts text at end of the log window instead of at the curser
-added option to join normal games
-added feature to change hunted ips while running (will also check if current ip is a new hunted ip)
-added feature to change game duration while running
-added feature where the bot will auto-rejoin on dropped game, and will continue hunting if unable to rejoin
-added feature where the bot will ask if you want to hold the current game if launched while already in a game
-added features to Hold Game and Abandon Game at the user's whims
-added rename all 'Diablo II' named windows option on the startup script
-improved error checking for game duration and game password (no more invalid characters)
-removed the useless winmove call
-removed the useless restore on start call
-removed the useless mousecoordmode call
-removed the now useless 'restore window on error' feature
-changed found game sound to not repeat endlessly
-renamed the 'Do not bring D2 window to front' to 'Run Minimized' so it is clearer
-changed create game detection method so after it will no longer attempt to create a game after getting kicked to the login screen
-changed game prefix and password errorchecking to not allow invalid characters
-altered Game Notification function to only do it if set to not minimized (would otherwise restore window even when set to minimized)
-removed 'Pause' hotkey for not supporting multi-windows

----

Update v1.8, 2009-02-02

-Added multi-window support. All windows must run minimized and have unique window names.
-Changed the way KCH asks for info (now one gui instead of several input boxes)
-Added restore and retry on error option
-Cleaned up code
-Added warning about redvex not working properly

----

Update v1.7, 2009-01-08

-Minor bugfix for users running with a resolution width of less than 1024

----

Update v1.6, 2008-12-27

-Added optional custom game password
-Added built in update feature
-Added startup GUI with readme button

----

Update v1.5, 2008-12-05

-unofficial patch for regular Diablo 2 v1.12a by PortalDeamon000
-fixed ingame detection bugs
-added option to mute the warning beeps

----

Update v1.4, 2008-09-30

-unofficial patch for Diablo 2 v1.12a by PortalDeamon000
-changed the ingame check function slightly
-works with D2loader (but not Origional Diablo 2 yet)

----

Update v1.3b1, 2006-08-26

- New GUI design.
- New Log window of hunting events, including timestamps.
- New Pause button, to stop the countdown to next game, mapped to "Pause" key on keyboard.
- New option of leaving the D2 window in the background (doesn't require bringing Diablo window to front to work).
- New option to automatically wait in a game if it sees a message "Diablo walks the Earth" or any sales of SOJs.
- Doesn't check bitmaps anymore for game state. Reads the D2 process memory directly for this information.
	Thanks to R1CH and Nomad for offsets to D2 memory.
- Better window-matching (uses 'classname=diablo ii' rather than matching title of window - thanks to PortalDeamon000).
- Now compatible with SOJ Reporter (and possibly D2Loader, though I haven't tested it and it's not suported)
- Recovers hunting if the game server crashes or there is a temporary connection problem (detects a return to lobby, and continues).
	However, if a server crashes, the character you're using will be unable to join games for several (5?) minutes.
- New startup sound (you can just delete the .wav files if you don't like them)

----

Update v1.2b1, 2006-05-16

- added functionality of checking that the lobby screen is up.
- added functionality of recovering from "Failed to join game" errors.

----

Update v1.1b6, 2006-05-10

- Reduced font size in display window; window can now be moved.
- Added fancy progress bar that can also be moved.
- Fixed bug introduced in v1.1b5 with randomized messages when sending a private message to the specified Bnet id.
- Tweaked time between games to try to prevent "Failed to join game" error between games - However, this is most likely
	due to packet loss or server problems. I have tested delay times as high as 10 seconds between games, and it seems to make no
	difference for me when the net is lossy. When BNET (or the connection to BNET) is laggy or lossy, "Failed to join game" errors occur.

----

Update v1.1b5, 2006-05-08

- Fixed another (subtle & rare) bug with IP identification logic: if both local and remote port numbers happen to be 4000,
	KCH was returning a CurrentIP of 0.
- Randomizes messages during anti-idling to avoid being easily detected as a robot (although nobody ever claimed this has happened).
- Upon failing to create a game, if you choose to continue, KCH now reminds you to prepare your D2 client as it does when you start KCH.

----

Update v1.1b4, 2006-03-15

- Fixed a bug with mouse and pixel coordinates - Snarg had everything "absolute" and this doesn't work if people have windows
	themes with large fonts (in the title bar, for example). Thanks to DeathBlade for point this out. Now everything
	is "relative to client window space" in AutoIt, so it should be OK.

----

Update v1.1b3, 2006-03-04

- Now randomizes the first letter of game name prefix to lessen chances of game name collisions, while keeping names easy to remember.
- New anti-idle strategy when a game is found: it now sends a battle.net message every 30 seconds and uses a tool-tip to give
	feedback to the user (instead of a dialog box). These Tool-tips aren't supposed to work in Win9x.
- Now detects if a found game drops during anti-idling (to avoid trying to anti-idle when you're no longer in a game).
- Added optional message recipient - if you specify a battle.net account name, the bot will /message that account giving information
	about game's name and password and IP. Useful if you play D2 on one CD-key and use another PC to run KissCloneHunter, but don't
	have easy access to it.
- Fixed another tricky bug with "TIME_WAIT" connections on port 4000 showing up and fooling the logic of the current IP. Thanks to
	Hate_IM on dcloneirc.net for reporting this!

----

Update v1.1b2, 2006-02-25

- fixed two bugs: 
  1. Snarg's code wasn't waiting for netstat command to complete before checking IP (problem on slower PCs, as the netstat
	command runs in a separate process and could take longer to complete) - My code now waits for temp file to be created by
	testing FileExists()
  2. Snarg's code was only checking first 20 lines of output from netstat (displayed "Current IP: 0" if you happened to have
	lots of connections on your PC) - My code now runs netstat -n | find "4000" command (shortening file), and reads entire file.
- added beeps, 5 seconds before timer expires, so you can let go of the mouse/keyboard, so as not to interfere with new game creation.

----

Update v1.1b1, 2006-02-16

- added simple timer countdown on display.
- updated display of "Trying to create game..."
- changed window title matching logic to "exact" - would sometimes match "Diablo II" web pages, as default match would be
	based on start of window only
- changed text of "Prepare client" dialog to be more explicit (i.e., open a character as opposed to select)
- re-positions D2 window upon reactivation
- replays the "Prepare client" dialog if game creation fails, so as to be sure that the user has set it into the correct state.

----

Improvements that 1.0b2 has over the original CloneHunter 2.2

- no more .ini file to configure
- no entering userid/password into third-party program or file
- no incredibly long game names and passwords
- no infinite loops that consume memory when a IP is found
- limited support for failed game creation ("Failed to join game", etc.)
- game duration is entered in seconds rather than milliseconds
- game name prefix is randomly generated but customizable
- enter as many IPs as you want (separated by commas)
- auto-detects the realm (not fully tested)
- attempts to anti-idle when hunted IP is found (not fully tested)
- window activation works now

----

Why KISS?

Kiss = keep it simple stupid

I was tired of using CloneHunter2.2 with all its kludginess, despite it being based on an excellent tool (Auto-It). So I
decided to redo it. Snarg was nice enough to distribute the .au3 (Auto-it3 file), and I'm also doing the same.
Check out http://www.autoitscript.com/autoit3/ - you will be impressed.

My .au3 *code* is not simpler. However, many things about how the program works are.

2006-01-14
Fuhrmanator@gmail.com
