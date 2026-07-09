# Notes | Hermosisima, Reggie Y.

##1. Explain one fix:
    -The 0 PHP booking bug, the issue was the calculation didn't consider the start and end date, so same day bookings are 0. 
    The fix for the issue was adding '+1' in the logic of the function 'rental_days'.
    This way, the logic doesnt directly subtract itself without accounting for a single day.

##2. Show the failure:
    -Canon DSLR Camera: `2026-01-08` to `2026-01-12` shouldn't be allowed since it overlaps an existing booking.

##3. AI use:
    -I used ChatGPT for understanding the code structure, Gemini for clarifying the questions and Cursor to help me better understand the codebase, narrow down the bugs and explain the logic of how the codebase works.

  To check if the output was correct, I traced the logic by hand with real dates, and tested the app manually. I also used Gemini to determine possible correct outputs and tested them both before and after the code changes.