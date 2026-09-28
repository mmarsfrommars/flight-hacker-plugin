---
name: flight-hacker
description: Find and compare practical low-cost flight options using current web research, nearby-airport routing, total-trip-cost analysis, evidence grading, and booking-timing context.
---

# Flight Hacker

Use this workflow whenever a user wants to optimize airfare or route planning.

The goal is not merely to find the lowest advertised fare. The goal is to identify the lowest realistically usable trip cost while clearly separating verified fares, estimates, nearby-date fares, and general market context.

## 1. Collect minimum trip constraints

If not already known, ask only for missing essentials:

- origin city or airport(s)
- destination city or airport(s)
- outbound date or date window
- return date or one-way
- number of travelers
- cabin class
- baggage needs
- flexibility on:
  - nearby airports
  - dates
  - overnight layovers
  - self-transfers
  - positioning trains/buses/flights

Do not ask for unnecessary details before starting research.

## 2. Search current options broadly

Search fresh sources and prioritize:

1. official airline websites
2. reputable flight metasearch engines
3. airline fare pages
4. nearby departure airports
5. nearby arrival airports
6. split-ticket combinations
7. self-transfer combinations
8. positioning flights, trains, or buses when materially useful

Search exact requested dates first.

Only after that, use nearby dates or generic monthly fare ranges as contextual evidence.

Never present a nearby-date fare as if it were available on the requested dates.

## 3. Evidence grading

Every fare or itinerary must be classified as one of:

### VERIFIED — EXACT DATES
A fare that can be confirmed for the exact requested travel dates.

### VERIFIED — NEARBY DATES
A real fare found on dates close to the requested dates, but not the exact dates.

### ESTIMATED
A fare inferred from current market information, fare calendars, indexed prices, or incomplete search results.

### MARKET RANGE
A generic current price range for the route, season, or month.

Never mix these categories without clearly labeling them.

If an exact fare cannot be verified, say so explicitly.

Do not invent exact prices.

## 4. Build comparable itineraries

For each realistic option, capture:

- airline(s)
- departure airport
- arrival airport
- routing
- number of stops
- total duration
- overnight layover if applicable
- ticket structure:
  - protected connection
  - separate tickets
  - self-transfer
- base fare
- currency
- fare evidence class
- baggage included
- baggage fees if known
- seat fees only if operationally relevant
- airport transfer cost
- positioning transport cost
- accommodation cost if the itinerary forces an overnight
- known visa/transit constraints when relevant
- operational risk notes

Do not automatically include optional extras that the traveler does not need.

## 5. Calculate True Trip Cost

Calculate:

TRUE TRIP COST =
base airfare
+ required baggage
+ required airport access
+ required destination transfer
+ positioning transport
+ required accommodation
+ other unavoidable transport costs

Do not include optional extras unless the user asks for them.

If a component cannot be verified, label it clearly as estimated.

If too many major components are unknown, do not give a falsely precise total.

Use:

"True cost not precisely calculable"

when appropriate.

## 6. Self-transfer analysis

For separate-ticket or self-transfer itineraries, clearly state:

- whether tickets are protected
- recommended transfer buffer
- airport change if applicable
- immigration/security re-clearance
- baggage re-check requirements
- overnight requirement
- what happens if the first flight is delayed or cancelled

Do not call a self-transfer "cheap" based only on airfare.

Compare its true cost and operational risk against protected itineraries.

## 7. Nearby-airport logic

Test nearby airports only when the full positioning cost and time are plausible.

For each positioning option, include:

- transport mode
- estimated positioning cost
- extra travel time
- whether an overnight becomes necessary
- whether the savings remain meaningful after all costs

Reject nearby-airport hacks when savings disappear after transport costs.

## 8. Hidden-city ticketing

Hidden-city ticketing may be explained as a pricing phenomenon, but do not present it as a default recommendation.

Clearly state relevant limitations such as:

- checked baggage normally cannot be used
- later itinerary segments may be cancelled
- irregular operations may reroute the traveler
- airline contract-of-carriage issues may apply
- frequent-flyer consequences may apply

Only include it when materially relevant to the user's question.

## 9. Booking-timing context

Use current market evidence and historical context only as supplementary guidance.

Do not claim there is a guaranteed "best day to book."

Distinguish between:

- current observed fare
- historical seasonal pattern
- promotional fare
- short-lived sale
- general booking-window guidance

If a sale has a stated deadline, highlight the deadline.

## 10. Required output structure

Always organize the final answer into the following sections.

### A. Exact-date verified options

Only include fares confirmed for the user's exact dates.

Table columns:

| Option | Route | Stops | Exact dates verified? | Base fare | Required extras | True trip cost | Evidence quality |

If no exact-date fare can be verified, say:

"No exact-date fare could be reliably verified from the available sources."

### B. Useful nearby-date or estimated options

Table columns:

| Option | Route | Fare observed | Date/evidence type | Estimated true cost | Why it matters |

Never merge this table with exact-date fares.

### C. Alternative routing checks

Include relevant:

- nearby airports
- positioning flights
- trains
- buses
- self-transfers
- alternate arrival cities

For each, state whether the saving survives the added cost and time.

### D. Decision thresholds

Do not declare one political-style "winner" or use vague superlatives.

Instead give objective thresholds such as:

- Lowest verified total cost
- Lowest estimated total cost
- Shortest practical itinerary
- Direct option within €X of cheapest
- Self-transfer only worth considering below €X

Thresholds must be justified by the observed data.

### E. What to verify before booking

List any unresolved items such as:

- exact fare availability
- baggage rules
- airport transfer cost
- overnight layover
- self-transfer protection
- visa/transit requirement
- cancellation/change terms

## 11. Language rules

Use precise wording.

Prefer:

"observed at"
"verified for"
"estimated at"
"nearby-date fare"
"market range"
"not confirmed for the exact dates"

Avoid phrases such as:

"this definitely costs"
"this is the best option"
"this will be cheaper"

unless the claim is directly supported by verified comparable data.

## 12. Source discipline

When using web research:

- cite current sources
- prefer airline and first-party sources for fare rules
- use metasearch for discovery, not as unquestioned truth
- distinguish indexed prices from bookable live fares
- identify when a fare may have changed since indexing

Never fabricate availability.

## 13. Practical comparison rule

Do not recommend a more complex itinerary merely because it saves a small amount.

When comparing:

- direct
- protected one-stop
- self-transfer
- positioning itinerary

show the actual price difference and extra travel burden.

Example:

"Self-transfer saves approximately €42 but adds 5 hours and unprotected connection risk."

This is more useful than calling one option "better."

## 14. Preferred final summary

End with a compact operational summary containing:

- best verified price actually found
- strongest nearby-date or estimated lead
- direct-flight reference price
- self-transfer threshold
- whether waiting or monitoring is reasonable

If exact-date fares remain unverified, explicitly say that the result is a research shortlist rather than a booking quote.
