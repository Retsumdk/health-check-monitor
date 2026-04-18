[![Build](https://github.com/Retsumdk/health-check-monitor/workflows/CI/badge.svg)](https://github.com/Retsumdk/health-check-monitor/actions)
[![TypeScript](https://img.shields.io/badge/typescript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Node.js](https://img.shields.io/badge/node.js-20-green?style=flat-square&logo=node.js&logoColor=white)](https://nodejs.org/)
[![MIT License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

# Health Check Monitor

[![CI](https://github.com/Retsumdk/health-check-monitor/workflows/CI/badge.svg)](https://github.com/Retsumdk/health-check-monitor/actions)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.3-blue.svg)](https://www.typescriptlang.org/)
[![Node.js](https://img.shields.io/badge/Node.js-20.x-brightgreen.svg)](https://nodejs.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Distributed health monitoring for microservices. Track service health, uptime, and response times across your infrastructure.

## Features

- **Distributed Monitoring** — Check health across multiple services and regions
- **Custom Health Checks** — Define custom endpoints and validation logic
- **Alerting** — Get notified when services go down
- **Dashboard** — View health status at a glance
- **Latency Tracking** — Monitor response times and P99 latencies

## Installation

```bash
git clone https://github.com/Retsumdk/health-check-monitor.git
cd health-check-monitor
npm install
npm run build
```

## Quick Start

```typescript
import { HealthMonitor } from './src';

const monitor = new HealthMonitor({
  interval: 30000,  // check every 30s
  timeout: 5000,     // 5s per check
});

monitor.addService('api', 'https://api.example.com/health');
monitor.start();
```

## Related Repos

- [service-discovery-client](https://github.com/Retsumdk/service-discovery-client) — Dynamic service discovery
- [audit-logger](https://github.com/Retsumdk/audit-logger) — Immutable audit trail
- [rate-limiter-middleware](https://github.com/Retsumdk/rate-limiter-middleware) — API rate limiting

## License

MIT License — see [LICENSE](LICENSE)
