# sq_cruise_ship

# Build

Using tweego to compile .twee files to html file:

`./tweego_win64.exe -o sq_cruise_ship.html src`

# Testing

Use Selenium IDE https://www.selenium.dev/selenium-ide to run the ./selenium_test.side file in chrome. This file runs through a basic playthrough to a certain point.

This does require updating the file to point to the fully qualified local path for the test to run by replacing "path/to/directory" in all locations in the file.

# Plans

## Must

need to DRY up the class reminder section:
`(DECK 7)</span></span><<elseif String.format("{0} {1} {2}, {3}"), GameDays[$gameDate.getDay()] isnot "Sun" and $gameDate.getHours() gte 11 and $gameDate.getHours() lt 13>><span class="fade-in-out"><span class="ad">CAPTAIN T CLASS 11-13 `

autopopup using the passage title in the popup itself is annoying. need to fix to decouple passage and file names from game experience

need to rename all the UntitledPassage files

Might need to burn this repo after a while and migrate to a new one to remove bad files from git history.

add a reminder on days with the stage events so they dont get missed

## Ideas

Extend reorganization of twee files into more directories

Will include basic save files within the repo at some point. Might use them for more easy automated testing. Might include a way to skip to later chapters by setting choices later.

Want to include ways to click the appointment reminder message to take us to the next appointment.

Make classes more forgiving in time, can skip 20 min to get to a class if needed
