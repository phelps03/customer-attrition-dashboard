# Brooks Customer Attrition Dashboard

Static, mobile-friendly dashboard for customer retention after first completed service.

## Data rules
- All 11 offices are included, including Nashville/Teddy's.
- Cohort start is each customer's earliest FieldRoutes appointment with status `Completed`.
- Active is the customer's current FieldRoutes Active status.
- Attrition tenure is calculated from true first completed service date to cancellation month, using the Sheet5 bands: 0-3, 3-6, 6-9, 9-12, 12-18, 18-24, and 24+ months.
- Inactive records without a usable cancellation month stay visible as `Cancellation date unknown` rather than being assigned to a band.
- The public `data.json` contains only aggregated counts. It contains no customer IDs, names, addresses, phone numbers, emails, notes, API keys, or tokens.

## Refresh
Regenerate `data.json` from the FieldRoutes API in a trusted environment, then publish the new aggregate file. Never put FieldRoutes credentials in this repository or browser code.
