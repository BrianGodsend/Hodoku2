# Changelog

All notable changes to HoDoKu are documented here.

---

## [2.3.5] – 2026-06-30

### Changed

- Aligned README build table; tightened markdownlint config

---

## [2.3.4] – 2026-06-30

### Changed

- Renamed repository from Hodoku2 to HoDoKu; updated internal project references

---

## [2.3.2] – 2022-06-26

### Changed
- Updated to work with JDK 18

---

## [2.2.0] – 2012-07-31

### Added
- `#204` ColorKu mode (thanks to ddyer and CCV)
- `#3486780` Complete ALS-Chain search in "Find All Steps"
- `#3476006` Improved keyboard handling
- `#3387327` Mouse click detection
- `#3480600` Larger fonts for visually challenged users
- `#3463520` "Auto Tab" feature
- `#3489431` Improved interoperability with SimpleSudoku
- `#3489725` Removed BrowserLauncher2 library dependency
- `#3454460` Save command
- `#3387347` Switching to "Show all candidates" now retains eliminations
- `#3510435` Clear cells using the mouse
- `#3515456` Locked candidates separation
- `#3520336` Reorganized preferences dialog
- `#3520334` Changed UI for saving Sudokus as images
- `#3515747` Deviations, filters, and alternate mouse mode
- `#3514371` Shade filter toggle buttons when no candidates are available
- `#3514367` Candidate highlight for filters
- `#3523432` Configurable line thickness for boxes
- `#3514351` Reduced puzzle difficulty for "hard" and "unfair"
- `#3527849` Save state of coloring cells/candidates

### Fixed
- `#3476976` Debug message written to console window in batch mode
- `#3492680` Inconsistent fish sorting (Finned/Sashimi)
- `#3513608` Comparison exception in AlsComparer
- `#3513603` "Find all steps" ignored ALS types
- `#3509643` Undo/Redo and all-steps error
- `#3513680` Problems displaying ALS-XZ
- `#3513851` Singles sorted wrongly in All Steps panel
- `#3509639` Deleting values from cells was broken
- `#3509637` All Steps could become out of sync
- `#3514467` `addSudokuToHistory()` could throw an exception
- `#3515379` Filter sets invalid candidate/value
- `#3516396` Filters and Hidden Singles conflict
- `#3514464` Changing maximum scores did not reset pre-generated puzzles
- `#3516415` Background generation request cancelled generation
- `#3521140` Setting a cell via context menu did not enable Undo
- `#3530975` Setting values in regions was broken

---

## [2.1.3] – 2012-01-19

### Fixed
- `#3475960` HoDoKu did not start when no default config file exists

---

## [2.1.2] – 2012-01-16

### Added
- `#3452538` Background colors can alternate
- `#3436698` Command line option `/sl` added
- `#3473994` OR instead of AND for filter (configurable)
- `#3463740` Additional info in All Steps view

### Fixed
- `#3467383` Exception when starting from `hodoku.jar`
- `#3453781` Exception when batch creating puzzles
- `#3454452` Pressing `Ctrl+C` in batch mode threw an exception
- `#3436963` Backdoor search was broken
- `#3425041` Could not always paste on macOS
- `#3454627` Volatile `anzFound` not updated atomically
- `#3432099` `Shift + numeric value` not working

---

## [2.1.1] – 2011-10-23

### Added
- `#3427511` When a single cell is selected, the cursor display disappears after 1 second (configurable)

### Fixed
- `#3427507` Brute Force solver broken in batch mode
- `#3427508` Template Set/Delete gave incorrect steps after a while
- `#3427509` A search for Kraken Fish could throw exceptions
- `#3427510` When candidates were colored they were not displayed correctly

---

## [2.1.0] – 2011-10-20

### Added
- `#3387351` New extended print dialog / booklet printer
- `#3387344` Simplified mouse mode
- `#2940096` HoDoKu is now portable
- `#2940101` / `#3011686` Puzzles are now created in the background
- `#3387345` Progress marker
- `#2990569` Tooltips for main frame
- `#3324082` Highlight more than one candidate
- `#3296914` Remove candidates via keyboard when a range of cells is selected
- `#2970905` / `#3144406` Reworked loading of incorrect puzzles
- `#2995579` Sped up creation of training puzzles
- `#2689169` Allow URs/HRs with missing candidates
- `#3387335` Fullscreen mode; hint pane and toolbar are now hideable
- `#3387341` Changed display of focus (configurable)
- `#3387355` Filter for bivalue cells
- `#3387356` Game mode as startup option
- `#3387357` Hint buttons in the toolbar
- `#3387359` "Solve up to" feature
- `#3394519` Coloring of cells with values is now configurable

### Fixed
- `#3098767` Create Sudoku window hangs
- `#3394539` Difficulty levels not stored between runs
- `#3387212` Example grids in "Print Solution" could be incorrect
- `#3303097` Fixed display of selected items under Nimbus look-and-feel
- `#3214361` Fixed errors when loading incorrect PM grids
- `#3134693` Hidden Pair incorrectly identified as Locked Pair
- `#3054092` Show deviations option was not remembered
- `#2954459` Arrows drawn incorrectly
- `#3387353` Set value in group of cells was broken

---

## [2.0.1] – 2010-04-14

### Added
- `#2974069` Import of givens into an existing grid
- `#2987128` Print option for solution paths

### Fixed
- `#2984538` XY-Chains not found

---

## [2.0.0] – 2010-03-11

### Added
- `#2834110` New mouse interface
- `#2940268` Selection of a region of cells using the keyboard
- `#2939789` Coloring candidates as well as cells
- `#2939792` Links to user manual, solving guide, and home page in Help menu
- `#2939800` Separate menu items for loading/saving configuration files
- `#2834095` `Shift+Ctrl+Cursor` jumps to the next highlighted cell when filters are applied
- `#2940105` Savepoints
- `#2940106` History of created puzzles
- `#2940098` Learning/Training mode
- `#2689174` Sort options in "All Steps" panel
- `#2689183` Step progress measure
- `#2689181` Backdoor searcher
- `#2953525` Additional display options for fish (`/vf`)

### Fixed
- `#2790208` UR results not optimal
- `#2834090` Invalid grids exported to clipboard as PMs treated empty cells incorrectly
- `#2834091` Result panels not updated correctly when an invalid grid is loaded
- `#2834085` "Find all steps" did not find BUG+1
- `#2946982` Position of horizontal divider bar now adjusted correctly
- `#2834087` Shortest XY-Chain not found
- `#2790209` Accelerators for difficulty levels did not work correctly
- `#2811672` Filters did not work correctly when "Show candidates" was unchecked
- `#2795464` Grouped Continuous Nice Loops could eliminate too many candidates

---

## [1.2.4] – 2009-05-08

### Added
- `#2772853` Use `Ctrl+Cursor` to go to next unsolved cell

### Fixed
- `#2762372` In coloring, not all possible eliminations were found
- `#2765903` Incorrect Siamese handling in Kraken search
- `#2765909` When searching for Kraken Fish, ALS were always used
- `#2788800` "Only one fish per elimination" did not return the smallest fish
- `#2788799` Search for all fishes found Basic Fish only when searching for Mutant
- `#2788798` Search for Franken/Mutant returned Basic Fish

---

## [1.2.0] – 2009-04-04

### Added
- `#2723180` Death Blossom solver
- `#2689196` "Enter game" renamed to "New Givens"; "Modify givens" added
- `#2689167` "Reset games" added; "Restart Game" reworked
- `#2690534` Type 1/Type 2 added to Kraken Fish output
- `#2533240` Dual 2-String Kites and Dual Empty Rectangles
- `#2691712` "One step only" option for fish search
- `#2689171` Support for Siamese Fish
- `#2690539` Selection of candidates in (Kraken) Fish search
- `#2512887` ALS Chaining redone to allow overlapping ALS (optional)
- `#2691742` Kraken Fish config added for general solver
- `#2723253` ALS overlapping is now configurable
- `#2723247` ALS nodes are now optional in Nice Loops/AICs and Forcing Chains/Nets
- `#2689864` Statistics options added for batch solve (`/vst`)
- `#2689186` Steps can be reordered via drag and drop

### Fixed
- `#2690494` All Steps panel not properly reset when a new puzzle is created
- `#2689165` Text for Template Set did not show the affected cells
- `#2689164` XY-Chain notation did not show start and end links
- `#2690582` All Steps panel quick links were not saved at program exit

---

## [1.1.0] – 2009-03-03

### Added
- `#2512895` Support for Kraken Fish
- Support for Turbot Fish
- `#2579893` ERs with only two cells in the ER are now found
- `#2512881` Sue de Coqs with the same additional candidate in both flanking sets are now supported
- `#2512876` Support for doubly linked ALS-XZ
- `#2512874` Changed chain ordering (size of ALS is now taken into account)
- `#2577506` Fish type (endo fins/cannibalism) added in console output
- New command line options: `/f`, `/bsa`, `/bsaf`, `/stdin`
- `#2634172` ALS nodes in Continuous Nice Loops are now handled
- "Find all steps" is now freely configurable

### Fixed
- `#2619238` ALS not displayed correctly in steps containing more than one chain
- `#2619244` ALS buddies handled incorrectly in chains
- `#2628375` Some AICs were not found
- `#2634176` AICs could overlap

---

## [1.0.0] – 2009-01-29

### Added
- Enhanced command line support: searching for puzzles with certain properties is now freely configurable (options `/c`, `/s`, `/lt`, `/so` added)
- Additional keyboard shortcuts
- `#2530890` More output options in batch processing (options `/vp`, `/vs`, `/vg`)
- `#2543821` Custom console for `hodoku-x.x.x.exe`
- `#2541410` `0` instead of `.` in export is now possible
- `#2536950` Window layout can be saved at shutdown

### Fixed
- `#2539619` Selecting tabs in right pane did not adjust menus
- `#2537408` Clicking a step after pressing F12 threw an exception
- `#2536944` Main window was too large
- `#2533245` Numpad did not work
- `#2531752` Reading the config file did not correctly adjust solver steps
- `#2530555` Forcing Chain notation was broken
- `#2512869` Nice Loop notation was incomplete for Continuous Nice Loops and AICs
- `#2512851` Background colors were not corrected when deleting solutions
- `#3510433` SummaryPanel errors

---

## [0.9.0] – 2009-01-15

Initial release of HoDoKu. Extensively tested and stable.
