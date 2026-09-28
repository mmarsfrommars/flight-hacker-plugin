# Product Spec — Flight Hacker v0.1

## Product goal
Turn the viral "cheap flight prompts" concept into a repeatable assistant workflow that produces a decision-ready comparison rather than a list of generic tips.

## MVP
The first version can be a skill-only ChatGPT/Codex plugin. It relies on the host product's web/search capabilities, so it does not need airline API keys to demonstrate the workflow.

### MVP capabilities
- cheap-flight search workflow
- official-site verification
- nearby-airport alternatives
- total-trip-cost calculation
- self-transfer / split-ticket warnings
- hidden-city explanation with contract-of-carriage caveats
- booking-timing context
- reusable 3-step search system

## Phase 2 — live travel APIs
Add a remote MCP app/backend when you want structured live inventory and automation.

Suggested provider-adapter interface:
- searchFlights(query)
- getFareDetails(offerId)
- searchNearbyAirports(location)
- estimateGroundTransport(origin, destination)
- createPriceWatch(query, threshold)

Keep providers behind adapters so you can swap commercial APIs without rewriting the assistant logic.

## Phase 3 — user accounts / alerts
- saved trips
- price thresholds
- email/push notifications
- currency preference
- baggage profile
- home/nearby airports

## Non-goals for v0.1
- purchasing tickets on behalf of users
- bypassing airline controls or fare restrictions
- guaranteeing price drops
- scraping sites in violation of their terms

## Core user inputs
- origin
- destination
- outbound date or range
- return date / one-way
- travelers
- cabin
- baggage
- flexibility flags

## Core output object
```json
{
  "search_timestamp": "ISO-8601",
  "currency": "EUR",
  "assumptions": [],
  "options": [
    {
      "route": "FCO-LHR-JFK",
      "airlines": ["Example Air"],
      "depart_at": "ISO-8601",
      "arrive_at": "ISO-8601",
      "stops": 1,
      "duration_minutes": 0,
      "headline_fare": 0,
      "baggage_cost": 0,
      "ground_transport_cost": 0,
      "other_required_cost": 0,
      "estimated_total": 0,
      "booking_source": "official|ota|metasearch",
      "booking_url": "",
      "self_transfer": false,
      "risk_notes": []
    }
  ]
}
```

## Ranking
Use separate transparent criteria rather than a mysterious global score:
- lowest all-in cost
- shortest practical duration
- fewest travel-friction points

## Privacy
Do not require passport numbers, payment-card data, or exact home address for searching fares. Store only the minimum needed for saved searches if accounts are added later.
