# Brooks Customer Attrition Dashboard

Static, mobile-friendly dashboard for customer retention after first completed service.

## Data rules
- Brooks offices only. Nashville is excluded because it is Teddy's Pest Solutions.
- Cohort start is each customer's earliest FieldRoutes appointment with status `Completed`.
- Active is the customer's current FieldRoutes Active status.
- The public `data.json` contains only aggregated counts. It contains no customer IDs, names, addresses, phone numbers, emails, notes, API keys, or tokens.

## Refresh
Regenerate `data.json` from the FieldRoutes API in a trusted environment, then publish the new aggregate file. Never put FieldRoutes credentials in this repository or browser code.
