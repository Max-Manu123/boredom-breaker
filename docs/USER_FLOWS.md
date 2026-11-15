# User Flows — Boredom Breaker

**Status:** Draft from current source.

## Flow A — Find an idea from home
1. User opens Home.
2. User understands the promise and sees discovery options.
3. User chooses Explore or a category.
4. User scans activity cards.
5. User opens an activity detail.
6. User reads the materials and steps.
7. User optionally saves the idea.

**Success:** user finds an activity they are willing and able to start.

## Flow B — Surprise Me
1. User selects Surprise Me.
2. App chooses an activity from the current category scope (currently all activities from Home).
3. Detail view opens.
4. User reviews the idea and optionally saves it.

**Review point:** consider whether random selection should account for duration, mood, energy, materials or prior dismissals. Do not add complexity without evidence.

## Flow C — Search and filter
1. User opens Explore.
2. User enters a search phrase.
3. User optionally selects a duration.
4. User optionally selects a category.
5. Results update.
6. User opens a result or clears the search.

**Success:** results match the user's intent and filters can be reset easily.

## Flow D — Saved ideas
1. User opens Saved.
2. App loads IDs from localStorage.
3. User opens a saved activity or removes it.
4. If no items remain, the empty state offers a path back to Explore.

**Success:** saved ideas remain available after refresh on the same browser.

## Flow E — Language switch
1. User selects EN or PT.
2. Interface labels update.
3. All content should remain understandable in the selected language.

**Known gap:** source currently switches many UI labels, but activity names, descriptions, steps, categories and difficulty values appear to remain English. Treat full content localisation as incomplete until verified and fixed.
