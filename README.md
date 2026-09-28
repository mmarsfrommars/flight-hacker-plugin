# Flight Hacker Plugin

A starter repository for turning a set of "cheap flight" prompts into a reusable ChatGPT/Codex plugin/skill.

The repository contains:
- a standalone plugin manifest in `.claude-plugin/plugin.json`
- the operational skill in `skills/flight-hacker/SKILL.md`
- a copy/paste master prompt in `docs/MASTER_PROMPT.md`
- an MVP / API expansion product spec in `docs/PRODUCT_SPEC.md`
- GitHub/import notes in `docs/GITHUB_SETUP.md`
- test prompts in `examples/TEST_CASES.md`

## What v0.1 does
It turns a broad travel request into a structured workflow: search current fares, compare official airlines and aggregators, check alternative airports/positioning routes, calculate all-in cost, warn about separate-ticket risks, and explain booking timing.

It also handles hidden-city ticketing conservatively: informational comparison only, with airline-contract and operational caveats.

## What it does NOT do yet
This starter does not include a live airfare API, ticket purchasing, scraping infrastructure, or user accounts. For structured live inventory, add a remote MCP/Apps SDK backend and commercial travel-data provider in a later phase.

## Quick start
Read `docs/MASTER_PROMPT.md` first. For ChatGPT plugin import, see `docs/GITHUB_SETUP.md`.

## Suggested repository name
`flight-hacker-plugin`

## License
Choose a license before making the repository public. MIT is a common option for a small open-source starter, but this repo intentionally does not impose one.
