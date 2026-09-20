How the logic works:
Persistence: The game saves to localStorage. If you close the browser and come back, it remembers when you started.
The Weekly Goal: Every time you whisper a thought, the weeklyCount goes up.
Check-In: The code calculates how many weeks have passed since the lastCheckIn. If the user vanishes for 3 weeks, the code will trigger 3 cycles of penalties.
Health Penalty: If weeklyCount is less than 7 when a week rolls over, Health drops by 20%. If health hits 0%, the egg becomes a "faded soul" and won't hatch.
Hatching: The "Hatch" button only triggers daysLeft === 0.
