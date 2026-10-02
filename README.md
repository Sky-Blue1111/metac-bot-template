# Forecasting bot runner

This repository only runs a forecasting bot for the Metaculus FutureEval tournaments.
The bot itself is kept in a private repository and is checked out at run time.

- `Forecast` runs every 10 minutes (an external scheduler plus a backup cron).
- `Test bot` runs the bot on the public `bot-testing-area` tournament only.
- Logs print question ids, counts and error types only; the `status` branch holds a
  counts-only `status.json`.

Every forecast is made by the code without human input; nobody edits, nudges or
approves a forecast before it is posted.
