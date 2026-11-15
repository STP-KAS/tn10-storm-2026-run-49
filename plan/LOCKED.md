> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · The lock. Written before any submit.

# Locked

- Network: Kaspa testnet-10 only. The desk node is not restarted.
- Pre-run 47's controller is not started. This run does not write that run's stop files.
- Pre-run 48's plan is not edited. Its payment process is not started again.
- No covenant hop sender, no KCC mint, no heavy lane.
- Payments: two processes, one key, disjoint coins, fee 100 sompi per gram. Signed-mass budget 1,690 grams until a sample says otherwise. Fee is that mass times 100. Each lane offers 1,520 a second. A met reading raises each lane to 2,027 for one more reading, then stop. A miss stops after the first reading.
- A coin may be reused in the same second. A lane spends only the coins it was dealt and the change it created. No second scan of the address.
- No 30-minute hold, no 8-minute pause, no clock return. Six full minutes are a reading. The run also stops if the bag cannot fund one more minute, or free space is under 150 GB, or the stop file is present.
- Do not arm if free space is under 160 GB, the node is not synced on testnet-10, the coin count is under 400, or the bag is under 8,000 tKAS.
- Kinds, only if the engine answers at the arm: tic-tac-toe quote-only, new match directories; flow at 2,000 after two confirmed coins; account at 100 and at 2,000 after two confirmed coins. Game gate: issuer coins 2 to 4 and at least 40 tKAS, operator coins 1 to 4 and at least 20 tKAS. No fifth coin of either.
- If the engine does not answer, the log says so and the payment half still runs.
- Submit-OK is not inclusion. Desk accept is the guest count.
- One node. A miss of a target is a later repo, not an edit of this lock.
