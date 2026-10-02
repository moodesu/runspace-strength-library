# The RunSpace — Exercise libraries

A static strength and movement library with responsive cards, desktop filter rail, collapsible mobile filters, a browser-local workout builder, workout player and printable workout sheets. Strength and Warm-ups & mobility are separate views. The latter offers search and filters for heart-rate raisers, mobility routines, targeted mobility, running drills and stretches. Videos open on demand with their source exercise explanations.

The strength export has 712 lesson records and 286 distinct videos with 285 available video descriptions. The warm-up export has 143 records, of which 142 were collected successfully: 114 distinct demonstrations with descriptions. Redwood Post Run Yoga Session remains unresolved and is not published. Repeated videos across course categories are shown once with combined categories.

See VIDEO_LINK_AUDIT.md and data/gokollab-import-audit.json for destination checks, excluded source pairings and coverage. Source descriptions are rendered as plain text. Slightly different descriptions across the two courses are retained in their respective contexts.

Sites serves dist/index.html via .openai/hosting.json. The existing Netlify repository serves the equivalent index.html from the root. Browser-local workouts remain separate for each origin.
