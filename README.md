# cryptools

## Jobs
- https://cryptojobslist.com/ (and follow https://github.com/ksaitor)
- https://www.paradigm.xyz/2021/09/the-community-garden-the-case-for-leaving-faang-companies-for-crypto/
- 
## Resources
- OpenZeppelin contracts wizard for plugging/playing with Ethereum standards
  - [Example walkthrough](https://www.linkedin.com/pulse/how-calculate-ethereum-gas-prices-keir-finlow-bates/)
- https://github.com/ConsenSys/ethereum-developer-tools-list
- https://github.com/dapphub/dapptools 
- https://github.com/dmihal
- web3 react: https://github.com/NoahZinsmeister/web3-react/tree/v6/example
- https://www.paradigm.xyz/2021/12/introducing-the-foundry-ethereum-development-toolbox/
- [web3js](https://web3js.readthedocs.io/)
- [alchemy web3js](https://www.npmjs.com/package/@alch/alchemy-web3)
- http://kernel.community/en/ : a bootcamp
- web3 buildspace

## Infrastructure
- https://tenderly.co/

## Topics of exploration/general:
- Gas estimation
- [Explanation](https://tracer.finance/radar/arbitrum-faqs/) of Arbitrum's gas situation

## Gas estimation
This comes down to two primary components: 
- gas price (most if not all web3 libraries provide this out of the box)
- estimation of contract call (via data payload)

There is plenty of traditional research being done in the space as well, on both gas estimation and optimization
- [GASOL](https://www.researchgate.net/publication/340692365_GASOL_Gas_Analysis_and_Optimization_for_Ethereum_Smart_Contracts)

https://ethereum.stackexchange.com/questions/27452/how-to-estimate-gas-cost

## Fundamentals
- eth2 and its roadmap (+ all research coming out of EF)
- scaling solutions
- mev
- EIP 1559 https://www.paradigm.xyz/2021/07/ethereum-reorgs-after-the-merge/

## Scaling ETH
- Optimistic rollups: https://research.paradigm.xyz/rollups
- Vitalik's guide to rollups: https://vitalik.ca/general/2021/01/05/rollup.html 
- [High-level medium article on Optimistic solutions](https://medium.com/privacy-scaling-explorations/an-introduction-to-optimisms-optimistic-rollup-8450f22629e8)
- Optimism's EVM equivalence: https://medium.com/ethereum-optimism/introducing-evm-equivalence-5c2021deb306
  - https://medium.com/ethereum-optimism/retropgf-experiment-1-1-million-dollars-for-public-goods-f7e455cbdca voting via quadratic voting
- [Optimistic vs ZK (by Matter Labs)](https://blog.matter-labs.io/optimistic-vs-zk-rollup-deep-dive-ea141e71e075)
  - [Accompanying comparison framework](https://blog.matter-labs.io/evaluating-ethereum-l2-scaling-solutions-a-comparison-framework-b6b2f410f955)
  - [The Graph integration for ZK](https://blog.matter-labs.io/thegraph-51c45d351029)
  - [zkEVM](https://zksync.io/zkevm/#what-is-zkporter)

## MEV
- https://hackmd.io/@flashbots/MEV-1559
- https://www.youtube.com/watch?v=rOVz7dOrGyY&t
- https://www.youtube.com/watch?v=7FY41j_uCLI
- mevintern
- https://arxiv.org/abs/2112.01472

## Collectives/DAOs
- w3b3.org
  - https://baton.art/
- https://daostack.io/

## Policy
- https://www.weforum.org/whitepapers/decentralized-finance-defi-policy-maker-toolkit

## Exploits/Liquidations
- https://cryptosec.info/defi-hacks/
- https://rekt.news/
- One more... escaping my mind rn
- [Aave May 2021 Retrospective](https://medium.com/gauntlet-networks/aave-protocol-liquidation-retrospective-may-2021-67c655fc1b31)
- Badger
- https://cointelegraph.com/tags/hacks

## Research
- [KEy-Loss Protection (KELP)](https://eprint.iacr.org/2021/289)
- Research onboarding: https://www.linkedin.com/posts/chalkiaskostas_ieee-xplore-full-text-pdf-activity-6878543519150145536-rsj4
- https://gauntlet.network/research/
- [Paradigm Research ](https://www.paradigm.xyz/writing/)
- [Gitcoin grants](https://gitcoin.co/grants/explorer?page=3&limit=12&me=false&sort_option=-amount_received&collection_id=false&network=mainnet&state=active&profile=false&sub_round_slug=false&collections_page=1&grant_regions=&grant_types=&grant_tags=&tenants=&idle=false&featured=true&round_type=false)
  - A true treasure trove of great projects
- AMMs:
  - [Allocation of Fungible Resources via a Fast, Scalable Price Discovery Method](https://arxiv.org/abs/2104.00282)
  - [Outstanding paper explaining AMMs](https://stanford.edu/~guillean/papers/cfmm-chapter.pdf)

## Opsec + Cryptography
- Library for multisigs (ECDSA, Bitcoin's Taproot): https://github.com/taurusgroup/multi-party-sig
- [Hardware wallet setups](https://docs.google.com/document/d/1kT5ITtr33T0kzR1dWjNPQNh7n74NvH_Lpm5i8lUzLe4/)
- https://frame.sh/
- Hardware wallets
  - GridPlus
  - Trezor
  - Ledger
  - KeepKey

## Interesting contracts
- [OpenDAO token](https://etherscan.io/address/0x3b484b82567a09e2588a13d54d032153f0c0aee0#code)
  - https://www.theopendao.com/
