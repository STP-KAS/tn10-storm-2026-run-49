> **Experimental. We are just trying this.** [Disclaimer](DISCLAIMER.md) · Kaspa Testnet-10 only; tKAS has no value.
>
> **This is a pre-run. Pre-run 49.** It is not the Wednesday run. It is not pre-run 1 to 48, and it does not edit their repos. A read does not start a runner.

# tn10-storm-2026-run-49

**Pre-run 49: two payment processes on disjoint coins, fee 100, aimed together at 3,040 a second, and the three vprog kinds if the engine is up.** The series name has no calendar date. The neuron stays [tn10-storm-2026-11-11](https://github.com/STP-KAS/tn10-storm-2026-11-11). This repo does not edit that repo. Pre-run 48 stays [tn10-storm-2026-run-48](https://github.com/STP-KAS/tn10-storm-2026-run-48).

> **Our own testing.** This is our own Kaspa Testnet-10 testing, run on our own machines and nodes. What these pages report is what we observed in this run; it is not a claim of how TN10 or Kaspa behave in general.

> **Last run of this stretch.** On 15 Nov 2026 we call it a day for now. Pre-run 49 is the last run of this stretch. This close is not a conclusion about Kaspa, and it is not advice.

| Field | Value |
|---|---|
| Target | A full minute whose two payment lanes sum to at least 2,200 submit-OK a second. One tic-tac-toe match accepted 8 of 8 during a payment minute, if the engine starts. One flow pass at 2,000 that is not an empty purse, if the engine starts |
| The change | One package after pre-run 48. Two processes instead of one. Each keeps its own coins. A coin may be reused in the same second. The offer is the pair, not a timed ladder. The kinds stay the three that already exist |
| Met or not met | **filled** on the table. Five full minutes, combined submit-OK 183,530, 190,827, 189,662, 181,172 and 181,032. All five are at least 2,200 a second. Three of them are over 182,400 and two are under, so 3,040 a second was not every minute. Zero rejects. The mempool field climbed from 173,092 to 905,883. The stop at 19:22:33Z is memory. The 4,053 offer was not raised. There is no sixth full minute. The engine was down in the payment window, so the tic-tac-toe match was after it: 8 of 8 at quote 216.16, at 19:52:41Z. Account at 100 completed a scripted pass while its sync line says behind. Account at 2,000 completed a scripted pass on a 20-second step after two shorter starts did not. Flow at 2,000 logged 2 activity submits. Those receipts are dev-mode. They are not real ZK receipts. Submit-OK is not inclusion |
| Retry count | 0. The next attempt is a new repo. This one is not resumed |
| Core tags | — |
| Status | done. Closed from the payment minute log and the kind phase lines. The plan pages are not edited. On 15 Nov 2026 we call it a day for now. This is the last run of this stretch |

Plan, lock, and the prediction are in [plan/PLAN.md](plan/PLAN.md), [plan/LOCKED.md](plan/LOCKED.md), and [plan/PREDICTIONS.md](plan/PREDICTIONS.md). Written before any submit. Those pages are not edited.

The minute bands are [counts/chain/MINUTES.md](counts/chain/MINUTES.md). The phase map is [counts/FINDINGS-MAP.md](counts/FINDINGS-MAP.md). The lessons are [logs/LESSONS.md](logs/LESSONS.md).
