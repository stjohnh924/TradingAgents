# Day Trader skills (vendored)

The `trader-*` folders here are the 11 project-local Claude Code skills from
[Jakeschincariol/day-trader-skill](https://github.com/Jakeschincariol/day-trader-skill)
(commit `3d0f4ef`, v2.0.0, MIT — see `DAY-TRADER-LICENSE`).

In Claude Code they show up as `/trader-scanner`, `/trader-news`, `/trader-entry`,
`/trader-exit`, `/trader-timemachine`, `/trader-budget`, `/trader-risk`,
`/trader-broker`, `/trader-alerts`, `/trader-analyst` and `/trader-pelosi`.

- Tools are standard-library Python 3.8+; nothing to install.
- They read free public data (Yahoo Finance, Nasdaq Trader, SEC EDGAR, House Clerk).
- SEC tools need `SEC_USER_AGENT="Your Name you@example.com"` or
  `sec_user_agent` in `trader/config.json`.
- Working files go to `trader/` in the repo root (git-ignored).
- Nothing places an order except `/trader-broker`, paper by default, and only
  after `/trader-risk` passes and you type yes. Not financial advice.

Upstream tests and fixtures were not vendored; see the upstream repo.
