> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · Kaspa Testnet-10 only. tKAS has no value.

# What this run is

Two payment processes, then the three kinds after the payment window. The game is tic-tac-toe and uses the priority quote. Account is tn10-runtime. Flow is tn10-flow. The payment class is simple payments at 100 sompi per gram. Submit-OK is not inclusion. A dev-mode receipt is not a real ZK receipt.

## Payments

The bands are [counts/chain/MINUTES.md](chain/MINUTES.md). The engine-down line is 19:22:05Z, reason wsl-list-timeout, while the 19:22 minute was still submitting. The payment stop is 19:22:33Z on memory. The 4,053 offer was not started.

## Game

The engine-up line is 19:51:03Z. The first guest loop that minute stopped on a refill before a match: the issuer count on that line is 1. The next loop, a fresh directory, confirmed one match at 19:52:41Z: submit-OK 8, accepted on the desk 8, quote 216.16, issuer 2 coins and 44 tKAS, operator 26.70 tKAS. The stop line is 1 match, 8 submit-OK, 8 accepted. That match is after the payment window. It is not the locked "during a payment minute" row.

## Account and flow

These lines are after the payment window. The phase log is the source.

- Account at 100. A top-up at fee rate 1,000 sent 1 coin. The ready line is 2 coins and 23.47 tKAS. The pass line lists genesis, init, two distributions, two deposits, transfer and withdraw. The sync field on that line says behind. The receipt field says dev-invalid. We do not call that settlement or inclusion.
- Account at 2,000. The first start logged no spendable coins, available 0. A top-up at fee rate 1,000 sent 1 coin. The ready line is 2 coins and 23.5 tKAS. The next start at the short step was partial: one distribution accepted, one rejected as already spent, one deposit, one deposit missing, one transfer, then a lane action that did not confirm. The coin field after that partial is 3 coins and 19.57 tKAS. The following short start logged the init guest as config already exists, two distributions, two deposits, the same lane stop, and an already-spent reject. A later start with a 20-second step completed the scripted list: genesis, init, two distributions, two deposits, transfer and withdraw. The init guest on that pass still says the config already exists. The receipt field says dev-invalid.
- Flow at 2,000. A top-up at fee rate 1,000 sent 2 coins. The ready line is 2 coins and 44 tKAS. The pass line says 2 activity submits. The receipt field says dev-invalid. We do not call that inclusion.

The top-up fee rate is the setup rate. It is not the pass fee. The pass fees are 100 and 2,000 as named on those lines.
