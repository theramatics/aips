# ARC-9: Incentivise weUSDC/UST pool with Astro

## Preamble

```
AIP#: 9
Title: Incentivise weUSDC/UST pool with Astro
Author(s): @MaxCallisto
Contributors: n/a
Tags: general, generator
Type: Generator
Category: Binding (Executable Purely On-Chain)
Status: Deferred
Date Proposed: 2022-03-28
Date Ratified:
Dependencies: n/a
Replaces: n/a
```

## Summary

Incentivise weUSDC/UST pool on Astroport to build up liquidity. The purpose of this proposal is to create a deep liquidity pool of weUSDC/UST to bring swaps from USDC to UST and vice versa from Curve Finance to Astroport.

## Abstract

The weUSDC/UST pool is currently available in Astroport with a shallow liquidity of $2mil. Compare this against the other UST-USDC pool in various chains:

1. Pangolin Exchange (Avalanche): $43mil
2. Excalibur Exchange (Fantom): $8.43mil
3. Saber (Solana): $67.6mil

Since Astroport is the only DEX with a stableswap invariant pool on Terra for now, this places Astroport in the prime position to solidify itself as the cheapest and deepest liquidity of USDC & UST swaps. This sentiment is resonated by Luke, the CTO of Delphi, in his [tweet](https://twitter.com/lukedelphi/status/1500546385367773190?s=20&t=muomBeW1T3qyA_WXkGpqOQ).

Although UST is the default stablecoin within Terra, attracting liquidity of other stables such as USDC, USDT, FRAX and DAI/MIM could make Astroport a primary DEX for many who believes that Terra is the ecosystem with the deepest liquidity for DeFi.

## Motivation

Although this could be speculative, but creating a deep stablecoin pool in Astroport may one day be useful should Astroport decides to build cross-chain via xAstro and allowing users swapping USDC to UST directly from the Ethereum chain as I've explained in [this Twitter thread](https://twitter.com/Theramatics/status/1506607155926896648?s=20&t=muomBeW1T3qyA_WXkGpqOQ).

As the trading APR for weUSDC/UST pool is approx. 2.5%, the pool should be aggressively incentivised for the first 3 months, with the renewal pass 3 months being subjected to the price of Astro 1 month before the expiry of the Astro emissions. As the trading APR improves alongside the price of Astro, the actual emissions beyond 3 months could be significantly lower. The reason for aggressively incentivising this pool is due to the fact that this pool is in direct competition with Anchor (before it's dynamic earn rate kicks in). As Anchor Earn drops, the need for aggressive emissions can be tapered down.

## Specification

Listing down various feedbacks I’ve received from various channels:

Target liquidity of $20mil may be too shallow
There are 3 types of USDC LP pools which will require deep liquidity
Incentives could originate from the Terra community pool in which rewards can be paid in Luna / UST
While I agree that a deep liquidity pool for USDC-UST will be beneficial for Terra, I would suggest to hold off incentives from the community pool until Retrograde / Reactor / Apollo goes live, where bribes can be paid with Luna or UST to direct emissions to these pools, thus, improving the efficiency of Astro votes / UST bribe. Astro emissions to the pool can be easily redirected if there voters are not keen on continuing on with the emissions to these pools, hence, I’d hold off this until the Convex-like protocols are launched.

As for the first 2 points, I do agree on incentivising all 3 pools to a target of $50mil value at a target APR of 18%. Since the Dynamic Rate for Anchor Earn poll has been passed, we can expect that in the first month, the APY for Anchor Earn will drop from 19.5% to 18%. Therefore, depositors will be looking for an alternative to deposit their UST.

With an Astro price of $2.35 at writing, I would propose the following:

USDC-UST Pools	Mth 1 Astro Emissions	Mth 2 Astro Emissions	Mth 3 Astro Emissions
weUSDC-UST LP	320,000	320,000	320,000
wpoUSDC-UST LP	320,000	320,000	320,000
wsoUSDC-UST LP	320,000	320,000	320,000
Total Emissions	960,000	960,000	960,000
With the above emissions, the estimated rewards APR will be revised to:

Liquidity in LP Pool	Astro APR
$10,000,000	90.2%
$20,000,000	45.1%
$50,000,000	18.0%
$100,000,000	9.0%
$200,000,000	4.5%
(estimated APR values assume that $ASTRO = $2.35)

To avoid further dilution to the 1st year’s emission of 100,000,000 tokens which currently emits 8.33mil Astro tokens per month, I propose to reduce the emissions for all pools listed below by 11.52% to accommodate for the 920k ASTRO emissions to the 3 stablecoin pools above.
Post 3 months, we might expect that Astro price has risen and Astral Assembly has gone live for gauge voting, the renewal of emissions can be decided by Astral Assembly.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
