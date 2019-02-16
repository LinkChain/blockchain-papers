## Blockchain Papers
Blockchain Papers List, Updated Weekly.
## Table of Contents
1. [Consensus](#consensus)
1. [Cryptography](#cryptography)
1. [Privacy](#privacy)
1. [Smart Contracts](#smart-contracts)
1. [Applications](#applications)


## Consensus
- **[The Bitcoin Backbone Protocol: Analysis and Applications](https://eprint.iacr.org/2014/765.pdf)**. Garay J, Kiayias A, Leonardos N. EUROCRYPT '15.
Bitcoin is the first and most popular decentralized cryptocurrency to date. In this work, we extract and analyze the core of the Bitcoin protocol, which we term the Bitcoin backbone, and prove two of its fundamental properties which we call common prefix and chain quality in the static setting where the number of players remains fixed. Our proofs hinge on appropriate and novel assumptions on the “hashing power” of the adversary relative to network synchronicity; we show our results to be tight under high synchronization.

Next, we propose and analyze applications that can be built “on top” of the backbone protocol, specifically focusing on Byzantine agreement (BA) and on the notion of a public transaction ledger. Regarding BA, we observe that Nakamoto’s suggestion falls short of solving it, and present a simple alternative which works assuming that the adversary’s hashing power is bounded by   1/3 . The public transaction ledger captures the essence of Bitcoin’s operation as a cryptocurrency, in the sense that it guarantees the liveness and persistence of committed transactions. Based on this notion we describe and analyze the Bitcoin system as well as a more elaborate BA protocol, proving them secure assuming high network synchronicity and that the adversary’s hashing power is strictly less than   1/2 , while the adversarial bound needed for security decreases as the network desynchronizes.
- [The Bitcoin Backbone Protocol with Chains of Variable Difficulty](https://eprint.iacr.org/2016/1048.pdf). Garay J. Kiayias A, Leonardos N. '16.
- [Analysis of the Blockchain Protocol in Asynchronous Networks](https://eprint.iacr.org/2016/454.pdf). Pass R, Seeman L, shelat a. EUROCRYPT '17.
- [On Trees, Chains and Fast Transactions in the Blockchain](https://eprint.iacr.org/2016/545.pdf). Kiayias A, Panagiotakos G. '16.
- "RSCoin": [Centrally banked cryptocurrencies](https://arxiv.org/pdf/1505.06895.pdf). Danezis G, Meiklejohn S. '15.
- [Anonymous Byzantine Consensus from Moderately-Hard Puzzles: A Model for Bitcoin](https://socrates1024.s3.amazonaws.com/consensus.pdf). Miller A, LaViola JJ Jr. '14.


## Cryptography
- [On Bitcoin as a public randomness source](https://pdfs.semanticscholar.org/ebae/9c7d91ea8b6a987642040a2142cc5ea67f7d.pdf). Bonneau J, Clark J, Goldfeder S. '15.
- [Distributed Cryptography Based on the Proofs of Work](https://eprint.iacr.org/2014/796). Andrychowicz M, and Dziembowski S. '14.
- [Scalable, transparent, and post-quantum secure computational integrity](https://eprint.iacr.org/2018/046.pdf). Ben-Sasson E, Bentov I, Horesh Y, Riabzev M. '18.





## Privacy
- [Zerocoin: Anonymous distributed e-cash from bitcoin](http://ieeexplore.ieee.org/iel7/6547086/6547088/06547123.pdf). Miers I, Garman C, Green M, Rubin AD. S&P '13.
- [Zerocash: Decentralized anonymous payments from bitcoin](http://ieeexplore.ieee.org/iel7/6954656/6956545/06956581.pdf). Sasson EB, Chiesa A, Garman C, Green M, Miers I, Tromer E, Virza M. S&P '14.
- "Monero": [CryptoNote v2.0](https://cryptonote.org/whitepaper.pdf). Saberhagen N. '13?
- [Rational Zero: Economic Security for Zerocoin with Everlasting Anonymity](http://fc14.ifca.ai/bitcoin/papers/bitcoin14_submission_12.pdf). Garman C, Green M, Miers I, Rubin A. FC '14.
- [Mixcoin: Anonymity for bitcoin with accountable mixes](https://eprint.iacr.org/2014/077.pdf). Bonneau J, Narayanan A, Miller A, Clark J, Kroll JA, Felten EW. '14.
- [TumbleBit: An untrusted Bitcoin-compatible anonymous payment hub](https://pdfs.semanticscholar.org/a4ce/62a44770a33d1a19b5553f080d4f12e9e55d.pdf). Heilman E, Alshenibr L, Baldimtsi F, Scafuro A, Goldberg S. '16.
- [Blindly Signed Contracts: Anonymous On-Blockchain and Off-Blockchain Bitcoin Transactions](http://fc16.ifca.ai/bitcoin/papers/HBG16.pdf). Heilman E, Baldimtsi F, Goldberg S. FC '16.
- [Coinshuffle: Practical decentralized coin mixing for bitcoin](http://crypsys.mmci.uni-saarland.de/projects/CoinShuffle/coinshuffle.pdf). Ruffing T, Moreno-Sanchez P, Kate A. ESORICS '14.
- [Quantitative analysis of the full bitcoin transaction graph](https://eprint.iacr.org/2012/584.pdf). Ron D, Shamir A. FC '13.
- [How Did Dread Pirate Roberts Acquire and Protect His Bitcoin Wealth?](http://fc14.ifca.ai/bitcoin/papers/bitcoin14_submission_2.pdf). Ron D, Shamir A. FC '14.
- "MoneroLink": [An Empirical Analysis of Linkability in the Monero Blockchain](http://monerolink.com/monerolink.pdf). Miller A, Möser M, Lee K, Narayanan A. '17.
- [Provisions: Privacy-preserving proofs of solvency for Bitcoin exchanges](https://eprint.iacr.org/2015/1008.pdf). Dagher GG, Bünz B, Bonneau J, Clark J, Boneh D. CCS '15.
- [Increasing Anonymity in Bitcoin](http://fc14.ifca.ai/bitcoin/papers/bitcoin14_submission_19.pdf). Saxena A, Misra J, Dhar A. FC '14.
- [Blindcoin Blinded, Accountable Mixes for Bitcoin](http://fc15.ifca.ai/preproceedings/bitcoin/paper_3.pdf). Valenta L, Rowan B. FC '15.
- [Hawk: The Blockchain Model of Cryptography and Privacy-Preserving Smart Contracts](https://eprint.iacr.org/2015/675.pdf). Kosba A, Miller A, Shi E, Wen Z, Papamanthou C. SP '16
- [Could Network Information Facilitate Address Clustering in Bitcoin?](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final11.pdf). Neudecker T, Hartenstein H. FC '17.
- [Blind signatures for untraceable payments](http://blog.koehntopp.de/uploads/Chaum.BlindSigForPayment.1982.PDF). Chaum D. CRYPTO '83.
- [Exchange Pattern Mining in the Bitcoin Transaction Directed Hypergraph](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final17.pdf). Ranshous S, Joslyn A, Kreyling S, Nowak K, Samatova N, West C, Winters C. FC '17.
- [Confidential Assets](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final41.pdf). Poelstra A, Back A, Friedenbach M, Maxwell G, Wuille P. FC '17.
- [Mixing Confidential Transactions: Comprehensive Transaction Privacy for Bitcoin](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final6.pdf). Ruffing T, Moreno-Sanchez P. FC '17.
- [Switch Commitments: A Safety Switch for Confidential Transactions](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final23.pdf). Ruffing T, Malavolta G. FC '17.
- [CoinParty: Secure Multi-Party Mixing of Bitcoins](https://www.martinhenze.de/wp-content/papercite-data/pdf/zgh+15.pdf). Ziegeldorf, J.H., Grossmann, F., Henze, M., Inden, N. and Wehrle, K. CODASPY '15.



## Smart Contracts
- "Ethereum": [A next-generation smart contract and decentralized application platform](https://www.weusecoins.com/assets/pdf/library/Ethereum_white_paper-a_next_generation_smart_contract_and_decentralized_application_platform-vitalik-buterin.pdf). Vitalik Buterin. '14.
- [Ethereum: A secure decentralised generalised transaction ledger](http://gavwood.com/paper.pdf). Wood G. '14.
- [Fair Two-Party Computations via Bitcoin Deposits](http://fc14.ifca.ai/bitcoin/papers/bitcoin14_submission_10.pdf). Andrychowicz M, Dziembowski S, Malinowski D, Mazurek Ł. FC '14.
- [Step by Step Towards Creating a Safe Smart Contract: Lessons and Insights from a Cryptocurrency Lab](http://fc16.ifca.ai/bitcoin/papers/DAKMS16.pdf). Delmolino K, Arnett M, Kosba A, Miller A, Shi E. FC '16.
- [EthIKS: Using Ethereum to audit a CONIKS key transparency log](http://fc16.ifca.ai/bitcoin/papers/Bon16a.pdf). Bonneau J. FC '16.
- "Oyente": [Making Smart Contracts
  Smarter](https://www.comp.nus.edu.sg/~loiluu/papers/oyente.pdf). Luu L, Chu DH, Olickel H, Saxena P, Hobor A. CCS '16.
- [The Ring of Gyges: Investigating the Future of Criminal Smart Contracts](http://www.initc3.org/files/Gyges.pdf). Juels A, Kosba A, Shi E. CCS '16.
- [Town crier: An authenticated data feed for smart contracts](http://delivery.acm.org/10.1145/2980000/2978326/p270-zhang.pdf?ip=46.176.188.9&id=2978326&acc=OA&key=4D4702B0C3E38B35%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35%2E594C525CFFA2AFAF&CFID=923932938&CFTOKEN=56121949&__acm__=1492299159_38039f3afa858f241818fdcf190e0200). Zhang F, Cecchetti E, Croman K, Juels A, Shi E. CCS '16.
- [A Smart Contract for Boardroom Voting with Maximum Voter Privacy](http://fc17.ifca.ai/preproceedings/paper_80.pdf). McCorry P, Shahandashti SF, Hao F. FC '17.
- [Constant-deposit multiparty lotteries on Bitcoin](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final39.pdf). Bartoletti M, Zunino R. FC '17.


## Applications
- [Blockstack Technical Whitepaper](https://blockstack.org/whitepaper.pdf). Muneeb A., Ryan S., Jude N, Michael F. '17
- [Storj A Peer-to-Peer Cloud Storage Network](https://storj.io/storj.pdf). Shawn W., Tome B., Josh B.,James P., Gordon H., Patrick G., Philip H., Chris P. '16
- [IPFS - Content Addressed, Versioned, P2P File System](https://github.com/ipfs/papers/raw/master/ipfs-cap2pfs/ipfs-p2p-file-system.pdf). Benet J. '15
- [BigchainDB: A Scalable Blockchain Database](https://www.bigchaindb.com/whitepaper/bigchaindb-whitepaper.pdf). McConaghy T, Marques R, Müller A, De Jonghe D, McConaghy T, McMullen G, Henderson R, Bellemare S, Granzotto A. '17


