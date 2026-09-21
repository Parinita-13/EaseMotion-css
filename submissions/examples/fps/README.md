# Puppeteer Scroll Animation FPS Benchmark

A headless Chrome performance benchmark runner designed to profile scroll animation frame rates (FPS), total bundle payload size, and script execution duration.

## Architecture & Features

- **Automated Scroll Profiling**: Simulates realistic viewport scrolling using Puppeteer.
- **Budget Threshold Assertion**: Enforces strict performance metrics; triggers CI step failures on threshold breaches.
- **Key Metrics Tracked**:
  - **FPS**: Minimum threshold $\ge 50$ FPS.
  - **Execution Time**: Maximum limit $\le 3000$ ms.
  - **Bundle Size**: Payload limit $\le 50$ KB.

## Quickstart

### Prerequisites
- Node.js 18+

### Setup & Execution

```bash
# Install dependencies
npm install puppeteer

# Run performance benchmark manually
node benchmarks/run-benchmark.js
