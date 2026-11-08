# Echowren 1.0 TEST
Native Android Simple Gako (Shinpurugako). These small boards are original generated layouts. Android 8+ (min 26), target 35. Package com.gg007.echowren.

## Rules
Simple Gako (Shinpurugako). Fill every cell with a positive number. Each N must count exactly N copies of that same number across its entire row and column, including its own cell once. Other digits do not block the count. No diagonal counting, connected-group requirement or Latin-square uniqueness rule. On a 3x3 board its cross has five cells, so only 1-5 can be valid. Tap an editable tile to cycle 1,2,3,4,5,blank. Gold clues stay fixed. Twelve original unique 3x3 clue boards and completed grids. Undo/reset/next/levels and saved number palette/fixed marks; clue color stays when marks are hidden.

## Download and status
https://mega.co.nz/#!Qdsl2YqI!T61qWcsZad__FQsh-cHEXOvkInAKQeFlkatDmyeQFQY
APK SHA256 88232b09427940b2c09fa2f641012116661a6719dfce31d9d40e86506ff83d64; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Exhausted all 1,953,125 full 1-5 assignments. An independent oracle constructs each cell cross as a set of row-or-column indices and counts matches, agreeing with production row/column frequency tables minus one. Exactly 40 full grids satisfy the rule; each of the twelve distinct clue boards has exactly one completion and all twelve solutions differ. Also checked 120,000 random/invalid boards, invalid array sizes/values, fixed clue locks, bounds, full cycle back to blank, solved lock and solve/undo/replay/reset. Archived portable generator reproduces levels.json and all-solutions.json; archived Java tests pass. Drawing adapter tests actual cell taps, fixed locks and gap taps, cycle-to-blank, reset/undo/replay/next/levels/menu/settings/privacy and saved palette/fixed marks/completion. Six drawing screens inspected, not phone screenshots. Phone runtime, performance and external-browser handoff QA remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Live 803-entry registry and semantic review of all 158 prior studio cards found no Simple Gako match. Degreegrove counts numbered edge-neighbors; Kenmeadow counts connected equal-digit group sizes; Ripplegrove spaces equal numbers. Echowren instead counts all equal digits on the whole row/column union, including itself once, with no blocking or connectivity rule. Known Simple Gako genre, not a global invention; inventor not established. Rules https://www.janko.at/Raetsel/Shinpurugako/index.htm . No source puzzle copied; original generated clue boards. Recovered repository corpus remains partial.

## Build
JDK 17 and Android SDK 35/build-tools35.0.0. python generate-levels.py reproduces levels.json. Board.java embeds generated fixed clues and solutions. javac -d /tmp/gako-test src/com/gg007/echowren/Board.java BoardTest.java and java -cp /tmp/gako-test com.gg007.echowren.BoardTest. bash build.sh creates an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Echowren runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Number palette, fixed marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon byte-equal to original. Menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/dkqqxf0zcnf7-echowren-source-archive, including exact cumulative 159-card studio and published catalog/studio sources/updater. Repository https://github.com/iLanis-agent/echowren holds README only; full Git source commit pending. Both website publications checked separately. No Pages settings change or Play rollout. November 8, 2026.
