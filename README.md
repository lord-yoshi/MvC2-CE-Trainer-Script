# MvC2-CE-Trainer-Script
A .ct file used with Cheat Engine 7.1 and Demul v0.7 111117 to add new functionality to Marvel vs Capcom 2 DC

Download the .ct file here: <a href="https://raw.githubusercontent.com/lord-yoshi/MvC2-CE-Trainer-Script/master/MvC2%20Trainer%20Script.CT">Right Click and Save Link As...</a>

-- Marvel vs Capcom 2 Cheat Engine Trainer Script

-- By Lord_Yoshi

-- Created some time in 2020

-- Used Cheat Engine 6.4, Demul 0.7 alpha 310715, and Marvel vs. Capcom 2 (USA) initially

-- Now switched to Cheat Engine 7.1, Demul 0.7 alpha 111117, and Marvel vs. Capcom 2 (USA)

-- Features include frame stepping, hitbox overlay, macro recording and playback, input log with frame counts, and many documented addresses

-- Feel free to do whatever you want with this script, but trying to sell it or claiming you created it would be rude.

--------------------------------------  ----------------------------------------
----------                     Table of Contents                      ----------
--------------------------------------  ----------------------------------------

-- 1. Shoutouts

-- 2. Setup

-- 3. Global Variables

-- 3a.  Constants

-- 3b.  Statics

-- 4. Functions

-- 4a.  Simple Memory Functions

-- 4b.  Hitbox Processing Functions

-- 4c.  Pausing Functions

-- 4d.  Macro Functions

-- 4e.  Input Display Functions

-- 4f.  Misc Functions

-- 5. Setup Code

-- 6. The End


--------------------------------------  ----------------------------------------
----------                        Shoutouts                           ----------
--------------------------------------  ----------------------------------------

-- SRK, jedpossum, https://forums.shoryuken.com/t/deconstructing-the-mvc2-dreamcast-cd/159481 for his mostly correct info

-- SRK, Jesuszilla, https://forums.shoryuken.com/t/mvc2-hitbox-viewer-data-tool-for-demul-0-7a310715/176626 for a decent, but messy base to start with that only received one reply in almost five years

-- ComboVid, Dammit, https://combovid.com/?p=3156 for some additional details on hitboxes

-- ZachD, Preppy, http://www.zachd.com/mvc2/ for the massive amount of MvC2 info in general

-- And so much more!


--------------------------------------  ----------------------------------------
----------                          Setup                             ----------
--------------------------------------  ----------------------------------------

-- Download and install Demul 0.7 alpha 111117 (http://demul.emulation64.com/)

-- Download and install Cheat Engine 7.1 (https://www.cheatengine.org/downloads.php) (I downloaded the raw files instead of running setup)

-- Acquire a Marvel vs Capcom 2 USA disk image

-- Use a Demul setup guide to find the missing files and get the emulator running

-- Map the Demul alternative control settings to the keyboard as follows:

-- P1: UP-W, DOWN-S, LEFT-A, RIGHT-D, A-V, B-B, X-Z, Y-X, LTRIG-C, RTRIG-N, START-M

-- P2: UP-T, DOWN-G, LEFT-F, RIGHT-H, A-J, B-K, X-U, Y-I, LTRIG-O, RTRIG-L, START-P

-- Once all preferred Demul settings are changed, run Cheat Engine

-- Using Cheat Engine, attach it to the Demul process (Click the monitor icon, then double click on the demul process), then load the Trainer Script cheat table (*.ct)

-- Run this lua script if prompted to, otherwise go to Table>Show Cheat Table Lua Script and click Execute Script

-- You should see the hitbox overlay and input log appear on the screen after a few seconds

-- If the buttons do not completely appear, the D3DHook has bugged out, so reload both Demul and CE and try again

-- Enjoy!

 <img src="https://raw.githubusercontent.com/lord-yoshi/MvC2-CE-Trainer-Script/master/Console%20Instructions.jpg" alt="Console Instructions"> 
