Check the status of Claude and GitHub services before a mob session.

Fetch https://status.claude.com/ and https://www.githubstatus.com/ using the WebFetch tool.

For each platform, list every service with its current status formatted as:
- ✅ OK — service name (if operational / no incidents)
- ❌ KO — service name (if degraded, partial outage, major outage, or incident)

Output the results grouped by platform with a header for each:

## Claude Status (status.claude.com)
...

## GitHub Status (githubstatus.com)
...

At the end, add a summary line:
- If all services are OK: "✅ All systems operational — good to go for mob session!"
- If any service is KO: "❌ Some services are degraded — check before starting mob session."
