> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · Kaspa Testnet-10 only. Written before any submit.

# Plan

Pre-run 48's follow-up was one payment process, 1,206 coins, fee 100, a coin reused in the same second. Full minutes sat near 1,710 to 1,770 submits a second. The 2,027, 3,040, and 4,053 offers were not reached. Zero rejects. While submits stayed near 1,710 a second the mempool climbed from about 17,941 to about 100,693, and it was near empty again within about two minutes after submits stopped. That run is not edited here. Its controller is not started again.

The question is whether a second process, on coins the first process does not spend, adds submit-OK above that one-process band. There is no time lock. A step ends when the minute log has the reading, or the bag cannot fund one more minute, or the disk abort trips. It does not end because a clock said 30 minutes, and it does not wait for an evening hour.

## What we read before this page

The check before this page, read-only, on the same payment key pre-run 48 left: 1,206 coins, 10,396.12 tKAS, signed mass 1,690, fee 169,000 sompi at 100 sompi per gram. The node was synced on testnet-10. Free space was 285.3 GB. The Docker engine did not answer. The account and flow binaries from the earlier build are still on the desk. The game image is still quote-only. No fourth kind is invented.

Finding 1 stays about 304 to 308 simple payments per block, about 3,040 to 3,080 a second. This run does not try to correct it. Submit-OK is not inclusion.

## Payments

Two processes. One fee, 100 sompi per gram. The mass is read from a signed sample and refreshed along the way. The fee is that mass times 100.

The coins are sorted once, at the start, and dealt even and odd. Lane 0 spends the even set and the change it creates. Lane 1 spends the odd set and the change it creates. Neither lane scans the address again. A coin may be spent again in the same second, from that lane's own change.

Each lane offers 1,520 a second, so the pair offers 3,040. There is no pause and no return phase on a clock. The first score is six full minutes after the partial minute in which the processes start.

- Met, on payments: any one of those six full minutes sums to at least 132,000 submit-OK across the two lanes (2,200 a second). If that happens, the same two processes raise the offer to 2,027 each, 4,054 together, for six more full minutes, and then they stop.
- Not met, on payments: all six full minutes sum to under 120,000 submit-OK (2,000 a second). The processes stop. The bag is not spent on a longer repeat of the same offer.
- A minute between those two lines is also a reading. The processes stop after the six minutes. The target is not met.

Disk abort is under 150 GB. Do not arm if free space is under 160 GB, the node is not testnet-10 and synced, the coin count is under 400, or the bag is under 8,000 tKAS.

## Kinds

The three kinds stay the three that exist. Tic-tac-toe is the exec-mode image and is quote-only. Account is `tn10-runtime`. Flow is `tn10-flow`. Those two carry the fee override. No fifth issuer coin and no fifth operator coin.

At the arm, one check asks the engine. If it answers, the game plays matches in new directories while the payments run, and flow is given two confirmed coins and one pass at 2,000. Account is given two confirmed coins and one pass at 100 and one at 2,000 if the binary starts. If the engine does not answer, the log says engine-down and those targets are not met because we did not start them. The payment half still runs.

- Met, on the game: one match with 8 accepted on the desk during a minute that also has payment submit-OK.
- Met, on flow: the 2,000 pass completes, or it logs a reject that is not an empty purse. An empty purse is our miss.

## What this page does not do

It does not restart the desk node. It does not start pre-run 47's controller. It does not write that run's stop files. It does not start a covenant hop line, a KCC mint, or a heavy lane. It does not spend the two storm keys that series leaves unused. It does not empty the mining address. The payment bag is the coins already on the payment key.
