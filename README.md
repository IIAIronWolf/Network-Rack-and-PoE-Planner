# Network Rack & PoE Planner

A browser-based, offline-capable tool for network engineers to visualize switch racks, power supplies, PoE budgets, and denied ports.

## Usage

Open [the planner](https://iiAironwolf.github.io/Network-Rack-and-PoE-Planner/) or download `index.html` and open it locally. The planner includes individual Copy buttons and a Copy all button for the following commands. Run them on the switch, then import a text capture containing the prompts and output:

```text
terminal length 0
show inventory
show switch
show environment power
show power inline
```

The first command disables pagination for the current CLI session. Include the switch prompt. Each capture generates a rack in stack-member order; drag members to match physical placement. Save project JSON, export CSV, or print a report.

## Privacy

The application processes imports in the browser, makes no application network requests, requires no credentials, and does not configure switches. No real customer captures are included in this repository. Download the HTML for offline use.

## Supported platforms

- Cisco Catalyst 9200 / 9200L (initial support)
- Additional vendors planned

## Roadmap

- PSU upgrade planning and capacity projections
- Multi-vendor CLI import adapters
- Improved reporting and rack layout

Upgrade candidates are advisory; verify PSU compatibility and electrical capacity before purchasing equipment.
