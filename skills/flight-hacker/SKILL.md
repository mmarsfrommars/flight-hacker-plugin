---
name: flight-hacker
description: Find and compare practical low-cost flight options using current web research, nearby-airport routing, total-trip-cost analysis, and booking-timing context. Use when the user asks for cheap flights, route alternatives, airport hacks, hidden-city explanations, or a repeatable flight-search workflow.
---

# Flight Hacker

Use this workflow whenever a user wants to optimize airfare or route planning.

## 1. Collect the minimum trip constraints

If not already known, ask only for missing essentials:
- origin city/airport(s)
- destination city/airport(s)
- outbound date or date window
- return date or one-way
- number of travelers
- cabin class
- baggage needs
- flexibility: dates, nearby airports, overnight layovers, self-transfers

Do not ask for details that are not needed to start searching.

## 2. Search broadly, then verify

Use fresh web research. Look for:
1. official airline websites and fare pages
2. reputable metasearch/aggregator results
3. nearby departure and arrival airports
4. split-ticket or self-transfer combinations when materially cheaper
5. rail/bus positioning legs when they reduce the total trip cost

Never present a stale fare as current. State the time/date of the search when practical.

## 3. Compare total trip cost, not headline fare

For each serious candidate, account for:
- base fare
- cabin/hand baggage
- checked baggage if required
- seat or mandatory booking fees if relevant
- airport transfer costs
- positioning train/bus/flight costs
- self-transfer buffer and overnight accommodation if needed

Prefer official airline booking links when the price difference is small.

## 4. Output a decision-ready shortlist

Return 3 to 6 options when possible. For each option show:
- routing and airline(s)
- departure/arrival times
- stops and total travel time
- fare found and what baggage is included
- estimated all-in cost
- booking source
- key tradeoff or risk

Then identify:
- cheapest practical option
- best value/time option
- simplest option

Do not call an option "cheap" if mandatory extras erase the apparent savings.

## 5. Nearby-airport and positioning logic

Check reasonable alternative airports at both ends. Include ground transport only when the savings remain meaningful after time and transfer costs.

Examples of useful patterns:
- fly from a nearby larger hub after a train ride
- arrive at a secondary airport and continue by rail/bus
- open-jaw itinerary when returning from a different city is cheaper
- separate tickets when the price advantage is substantial and the connection buffer is safe

Explicitly label self-transfers and separate-ticket risk.

## 6. Hidden-city ticketing

If the user asks about hidden-city ticketing, explain how it works and surface examples only as informational comparisons. Clearly warn that:
- it may violate an airline's contract of carriage or loyalty-program rules
- checked baggage normally continues to the ticketed final destination
- irregular operations can reroute the traveler past the intended stop
- skipping one segment can cause later segments on the same ticket to be cancelled
- it is generally unsuitable for round trips, checked bags, tight schedules, or loyalty-sensitive travelers

Do not describe it as "safe" or guarantee that an airline permits it.

## 7. Booking timing

When asked when to book:
- use current route/season context and any reliable historical pricing data you can find
- present a range or strategy, not a fake exact prediction
- distinguish high-demand periods, holidays, major events, school breaks, and low season
- recommend price alerts when uncertainty is high

## 8. Repeatable 3-step user workflow

When the user asks for a reusable system, give this compact process:

Step A — Discover: search flexible dates, nearby airports, and multiple sources.
Step B — Verify: confirm the best candidates on the airline's site and compute all-in cost.
Step C — Decide/Watch: book when the fare meets the user's threshold or set an alert if it does not.

## 9. Quality rules

- Never invent a live price, schedule, airline policy, or availability.
- Label estimates versus verified prices.
- Mention currency and whether taxes are included.
- If a fare comes from an OTA, note that post-booking support may differ from direct airline bookings.
- For separate tickets, recommend a generous buffer and explain that missed-connection protection may not apply.
- Keep the answer compact enough to act on, but include the assumptions used.
