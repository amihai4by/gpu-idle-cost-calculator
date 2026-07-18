# GPU Idle-Cost Calculator 💸

**[→ Open the calculator](https://amihai4by.github.io/gpu-idle-cost-calculator/)** — free, no signup.

Most Kubernetes GPU fleets waste **60–70% of their spend** on allocated-but-idle
cards. This is a tiny, single-page tool that turns that into a number: enter your
fleet size, GPU type, and average utilization → see your **annual idle-cost** and
how much you'd **reclaim** by raising utilization.

## Why utilization is the number that matters
A GPU costs the same at 100% or 0% — you pay for the *allocation*, not the work.
So utilization is a direct multiplier on real cost: a fleet at **30% utilization
pays 3.3× per useful GPU-hour** versus one at 100%. That gap is where most GPU
budgets quietly leak.

## How to actually cut it
- **Measure** per-GPU utilization (DCGM → Prometheus → Grafana)
- **Share** GPUs (time-slicing) or **partition** them (MIG)
- **Quota** to stop hoarding · **Spot** for interruptible work · **Reclaim** idle allocations

Copy-paste Kubernetes packs that do each of these:
- [GPU Monitoring Starter Pack](https://probizgen.gumroad.com/l/xxnqbt) — see the idle 70%
- [GPU Cost-Optimization Pack + Production vLLM Serving](https://probizgen.gumroad.com)

## Keywords
gpu cost calculator · kubernetes gpu cost optimization · idle gpu waste · gpu
utilization · h100 a100 cost per hour · reduce gpu costs · gpu finops · mig
time-slicing · llm inference cost

---
*Free tool, MIT-friendly, nothing tracked. Prices shown are editable list rates — use your own.*
