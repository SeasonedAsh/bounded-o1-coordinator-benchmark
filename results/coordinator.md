---

## 🔧 Hardware

- **Intel i7-4930K (2013)**  
- 6 cores @ 3.40 GHz  
- No GPU  
- Node.js runtime

---

## 📊 Summary (Extracted From JSON)

- **Throughput:** 2,533,436 cycles/sec  
- **Avg Latency:** 0.169 µs  
- **P50:** 0.200 µs  
- **P95:** 0.200 µs  
- **P99:** 0.300 µs  

### Memory

- Start: 5.34 MB  
- End: 8.76 MB  
- **Total drift:** 3.41 MB over 100M cycles

### Patterns

- SYSTEM_ACTIVE: 1,366,426  
- GROW_CACHE: 4,078  
- SYSTEM_IDLE: 2  
- No overload, no wanderers

---

## 🧪 Method

A scheduler was executed for **100,000,000 state-transition cycles** using mixed
task patterns. Metrics were recorded for:

- latency distribution  
- memory drift  
- stable pattern equilibrium  
- overload detection  
- throughput under continuous load  

The JSON file contains the raw results with no post-processing.

---

## ❓ Why Share This?

The notable part of this benchmark is not the throughput, but the **absence of
degradation**:

- no increasing latency  
- minimal memory drift  
- zero overload events  
- no oscillation under mixed-pattern load  

These are properties typically associated with kernel-level O(1) schedulers or
ring-buffer architectures rather than userland runtime environments.

This repository is shared for discussion, validation, and critique.

---

## 📝 Files

- `benchmark.md` — deeper explanation + context  
- `results/coordinator-1765466509579.json` — raw benchmark  
- `LICENSE` — MIT License  

---

## 🔗 Discussion

If you'd like to comment, a Hacker News discussion thread will be linked here
after submission.

---

MIT License  
