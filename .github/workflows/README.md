# Tenki Runner Benchmark

A hands-on, buyer's-eye test of [Tenki Runners](https://tenki.cloud/products/runners) versus GitHub-hosted runners.

**Question:** If I were a customer, would switching one `runs-on:` line actually make my builds faster and cheaper?

## The test
- **Workload:** a clean release build of [ripgrep](https://github.com/BurntSushi/ripgrep) v14.1.1 (a real Rust project, no cache).
- **Runners (same size on both sides):**
  - GitHub `ubuntu-latest`: 2 vCPU, $0.006/min list price
  - Tenki `tenki-standard-small-2c-4g`: 2 vCPU, $0.004/min
- **Runs:** 3 per runner, launched together, so one slow run doesn't skew the result.

## Results

| Runner | Run 1 | Run 2 | Run 3 | Average build | Total job time | Cost per job |
|---|---|---|---|---|---|---|
| GitHub ubuntu-latest | | | | | | |
| Tenki small 2c-4g | | | | | | |

**Cost per job** = total job minutes (rounded up for GitHub, per second for Tenki) × rate.

## What I noticed as a customer
- Setup time and friction:
- Anything confusing:
- What I'd tell a prospect:

## Pricing sources
- [Tenki pricing](https://tenki.cloud/docs/pricing)
- [GitHub Actions runner pricing](https://docs.github.com/billing/reference/actions-runner-pricing)
