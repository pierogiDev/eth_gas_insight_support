# ETH Gas Insight Support

ETH Gas Insight is a web service for Ethereum users who want to avoid overpaying gas.

This repository explains the project, its roadmap, known issues, and how donations will be used to keep the service running and improving.

## Site Overview

ETH Gas Insight provides gas price analysis and timing context for Ethereum users. The service focuses on making recent gas conditions easier to understand through a simple top-level summary and detailed charts for users who want deeper context.

Main site:

- https://ethgasinsight.info

Current focus:

- 24h, 7d, and 30d gas price analysis.
- Quick gas timing summary with `Cheap`, `Normal`, and `Expensive` status.
- Median, percentile, distribution, heatmap, block utilization, and transaction gas views.
- UTC-based time display for consistent bucket comparison.
- Public web UI backed by an Ethereum node and precomputed backend data.

## Development Roadmap

- Improve the top-level gas timing summary so non-technical users can understand current gas conditions faster.
- Add clearer explanations for advanced metrics such as percentiles, buckets, outliers, and block utilization.
- Improve mobile layout and chart readability.
- Add more historical context for recurring gas patterns.
- Improve backend refresh reliability and monitoring.
- Reduce infrastructure cost and deployment time.
- Add public status notes for data freshness and backend sync progress.

## Known Issues

- Some charts depend on backend precomputed tables and may lag briefly while refresh jobs are running.
- Mobile chart interactions can be harder to use than desktop interactions.
- Gas conditions can change quickly, so all indicators are informational and not guaranteed timing advice.
- Some advanced charts require Ethereum gas knowledge to interpret correctly.
- API availability depends on the home-hosted backend, network connectivity, and tunnel/proxy health.

## Changelog

### 2026-05-05

- Added `ETH Gas Now`, a quick gas timing summary card.
- Added a visual separation between quick timing context and advanced gas analysis.
- Added About page audience messaging.
- Improved CORS settings for Vercel, LAN, and VPN access.
- Added a frontend-only plain Docker deploy script.

## How Donations Will Be Used

Donations will be used to support:

- Ethereum node storage and hardware upgrades.
- Electricity and network costs for running the backend infrastructure.
- Backup storage and operational monitoring.
- Domain, DNS, tunnel, and hosting-related costs.
- UI improvements, documentation, and accessibility work.
- Time spent maintaining data freshness, fixing bugs, and improving reliability.

## Screenshots

Screenshots will be added under [`screenshots/`](screenshots/).

Suggested screenshots:

- Gas page top summary.
- Gas price trend chart.
- Detailed gas analysis section.
- Mobile view.
- About page.

## Contact

For questions, bug reports, or support-related messages, please use GitHub Issues in the main project repository or contact the project maintainer.

Main project repository:

- https://github.com/pierogiDev/eth_gas_insight

## GitHub Sponsors

Support development through GitHub Sponsors:

- https://github.com/sponsors/pierogiDev

## Disclaimer

ETH Gas Insight provides informational gas analysis only. It is not financial, legal, trading, or investment advice.
