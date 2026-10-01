# CallCrew proof of work

Two small tools built by David Hackett as part of a Founder's Associate application to CallCrewAI. Not an official CallCrew project.

- **`/tracker`** is the Missed-Call Audit. It lists 49 Limerick trades businesses (`tracker/businesses.json`, taken from numbers they advertise publicly) and logs each call by round: weekday working hours, weekday evening and Saturday morning. Outcomes, callbacks, podcast-guest answers and notes are saved in the browser's `localStorage` on the device you use, and can be exported as CSV.
- **`/calculator`** is the Missed Call Meter. It works out the revenue a trades business loses a year from missed calls, using inputs the owner sets.
- **`/`** is a short landing page linking the two.

## Run locally

It's plain static HTML with no build step:

```
npx serve .
```

## Deploy

Import the repo into Vercel with the framework preset set to "Other". There's no build command, and the output directory is the repo root.

## Notes

- Call results never leave the device unless you export them. Use one phone or browser for the whole audit, and export a CSV after each round.
- Registers such as Safe Electric ask that their listings not be used for marketing, so they're only used to confirm a contractor is legitimate.
