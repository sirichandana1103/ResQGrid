# ResQGrid prototype plan

## Product and demo scope

Build a responsive browser prototype called ResQGrid, separate from TrustSignal. It will demonstrate four connected areas: a citizen report form, a coordinator command centre, a volunteer task view, and a supplies/resource view. The demo will include sample flood, cyclone, landslide, and road-block reports from more than one Indian region. Users can add sample reports, review them, see possible duplicates, assign demo volunteers and supplies, update task progress, search and filter the queue, and view summary counts.

This ZIP is a front-end prototype only. It will use fictional sample data and browser-local state. It will not include working accounts, a FastAPI server, Supabase storage, real AI/ML, GPS capture, image analysis, live alerts, or emergency dispatch. Text-based suggestions will use simple rules and must be labelled as demo suggestions. Map markers will be marked as practice data. These limits will be stated in the app and README.

## Design direction

Use the user's minimal editorial enterprise-tech style: warm off-white background with a faint gray grid; near-black text; large bold sans-serif headings; bright orange for the brand, main buttons, and selected states; white cards with fine gray borders and soft corners; small uppercase labels; restrained shadows; simple line icons; and a spacious responsive layout. Keep priority colors separate from the brand: red-orange for high, amber for medium, and muted blue for low. Use plain English in all labels and messages.

## Implementation approach

Use React, Vite, and TypeScript. Keep the app static and use browser-local state so the main demo workflows work without accounts or credentials. Keep sample records, demo rules, UI components, and CSS in separate files. The map panel will use a clearly marked practice layer; no report will be shown as live or verified. Provide a reset action for the sample data and CSV export for the demo queue.

## Main files

- `src/App.tsx` — app shell, navigation, and selected module.
- `src/data/demoData.ts` — fictional incident, report, volunteer, resource, and task records.
- `src/lib/demoLogic.ts` — simple category, duplicate, and priority suggestions marked as demo rules.
- `src/components/` — reusable cards, labels, and map/diagram pieces.
- `src/styles.css` — responsive editorial theme and priority colors.
- `README.md` — run instructions, demo boundaries, and future backend notes.
- `public/manus-routes.json` — route title for the preview.

## Build, check, and ZIP

Use the pinned pnpm version. From the project folder, install with `pnpm install --frozen-lockfile`, run `pnpm dev` to use the local preview, run `pnpm check`, `pnpm test`, and `pnpm build`, then package the source as `resqgrid-prototype.zip`. Include source, lockfile, README, and needed public files. Exclude `.git`, `node_modules`, build output, and local secrets. Do not publish the site unless asked.