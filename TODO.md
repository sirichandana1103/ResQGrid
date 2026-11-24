# ResQGrid prototype — ToDo

## Citizen report form and status view — complete
- Let a citizen enter an incident type, place, region, short description, and number of people affected. Let them choose an optional photo file in the browser, but do not upload it or claim that it was analyzed.
- Show the submitted report in the demo with a simple status so a user can see the reporting flow.
- Do not claim that login, phone verification, or automatic GPS is active. Use practice data only.

## Coordinator report review and demo suggestions — complete
- Show reports in one review queue with their place, time, type, status, and priority band.
- Show simple demo suggestions for category, possible duplicate, and urgency. Label them as suggestions, do not merge reports automatically, and let a person choose the review action.
- Let the coordinator mark a report checked, request more information, or dismiss a practice report. These actions change the demo status only.

## Volunteers, supplies, and task progress — complete
- Show demo volunteers, their skills and availability, and their assigned tasks.
- Let a volunteer accept or decline a demo task and update its progress.
- Show demo supplies and shelters and let a coordinator make a sample assignment. Do not send a real team or change real inventory.

## Regional overview and simple analytics — complete
- Show practice incident markers for more than one region and hazard type. Clearly mark the map and every marker as practice data, not a live emergency map.
- Show counts from the sample records for review, reports, volunteer availability, supplies, and task progress.
- Let users search and filter the practice report queue and export its sample rows as CSV.

## Clear, responsive design and source ZIP — complete
- Use the user's warm off-white, subtle grid, near-black text, orange brand accents, white cards, thin borders, simple icons, and spacious responsive layout.
- Keep priority colors distinct: red-orange for high, amber for medium, and muted blue for low.
- Use short, plain-English labels and keep practice-data warnings visible on desktop and mobile.
- Include setup, build, test, and safety notes in README.md. Package source and required public files as a ZIP; exclude dependencies, build output, Git data, and secrets.

## Prototype limits — not implemented
- No live emergency reports, real AI or image analysis, accounts, GPS capture, backend, Supabase database, or emergency dispatch.
- The sample workflow runs in the browser only. Real use needs approved backend, privacy, security, and disaster-response processes.
