## Blockchain Papers
Blockchain Papers List, Updated Monthly.
## Table of Contents
1. [Consensus](#consensus)
1. [Cryptography](#cryptography)
1. [Privacy](#privacy)
1. [Smart Contracts](#smart-contracts)
1. [Applications](#applications)


## Consensus
### 1. Byzantine [The byzantine generals problem](https://www-inst.eecs.berkeley.edu/~cs162/sp16/static/readings/Original_Byzantine.pdf).Lamport L, Shostak R, Pease M. ACM Transactions on Programming Languages and Systems (TOPLAS), 1982, 4(3): 382-401. 
Abstract: Reliable computer systems must handle malfunctioning components that give conflicting information to different parts of the system. This situation can be expressed abstractly in terms of a group of generals of the Byzantine army camped with their troops around an enemy city. Communicating only by messenger, the generals must agree upon a common battle plan. However, one or more of them may be traitors who will try to confuse the others. The problem is to find an algorithm to ensure that the loyal generals will reach agreement. It is shown that, using only oral messages, this problem is solvable if and only if more than two-thirds of the generals are loyal; so a single traitor can confound two loyal generals. With unforgeable written messages, the problem is solvable for any number of generals and possible traitors. Applications of the solutions to reliable computer systems are then discussed.

### 2. FLP [Impossibility of Distributed Consensus with One Faulty Process](https://apps.dtic.mil/dtic/tr/fulltext/u2/a132503.pdf)  Fischer M J, Lynch N A, Paterson M S. Journal of the ACM, 1985, 32(2): 374:382
Abstract: The consensus problem involves an asynchronous system of processes, some of which may be unreliable. The problem is for the reliable processes to agree on a binary value. We show that every protocol for this problem has the possibility of nontermination, even with only one faulty process. By way of contrast, solutions are known for the synchronous case, the Byzantine Generals problem.

### 3. VR [Viewstamped replication: a new primary copy method to support highly-available distributed systems](http://www.cs.princeton.edu/courses/archive/fall11/cos518/papers/viewstamped.pdf) Oki B M, Liskov B H. In: Proceedings ofProceedings of the 7th Annual ACM Symposium on Principles of Distributed Computing.Toronto, Ontario, Canada: ACM, 1988. 8:17
Abstract: One of the potential benefits of distributed systems is their use in providing highly-available services that are likely to be usable when needed. Availabilay is achieved through replication. By having inore than one copy of information, a service continues to be usable even when some copies are inaccessible, for example, because of a crash of the computer where a copy was stored. This paper presents a new replication algorithm that has desirable performance properties. Our approach is based on the primary copy technique. Computations run at a primary. which notifies its backups of what it has done. If the primary crashes, the backups are reorganized, and one of the backups becomes the new primary. Our method works in a general network with both node crashes and partitions. Replication causes little delay in user computations and little information is lost in a reorganization; we use a special kind of timestamp called a viewstamp to detect lost information. 

### 4. Paxos[The part-time parliament](https://computerarchive.org/files/mirror/www.bitsavers.org/pdf/dec/tech_reports/SRC-RR-49.pdf)Lamport L. ACM Transactions on Computer Systems, 1998, 16(2): 133:169.
Abstract: Recent archaeological discoveries on the island of Paxos reveal that the parliament functioned despite the peripatetic propensity of its part-time legislators. The legislators maintained consistent copies of the parliamentary record, despite their frequent forays from the chamber and the forgetfulness of their messengers. The Paxon parliament's protocol provides a new way of implementing the state-machine approach to the design of distributed systems--an approach that has received limited attention because it leads to designs of insufflicient complexity.

### 5. PBFT [Practical Byzantine fault tolerance](https://www.usenix.org/legacy/events/osdi99/full_papers/castro/castro_html/castro.html)Castro, Miguel, and Barbara Liskov.1999.
Abstract: This paper describes a new replication algorithm that is able to tolerate Byzantine faults. We believe that Byzantine-fault-tolerant algorithms will be increasingly important in the future because malicious attacks and software errors are increasingly common and can cause faulty nodes to exhibit arbitrary behavior. Whereas previous algorithms assumed a synchronous system or were too slow to be used in practice, the algorithm described in this paper is practical: it works in asynchronous environments like the Internet and incorporates several important optimizations that improve the response time of previous algorithms by more than an order of magnitude. We implemented a Byzantine-fault-tolerant NFS service using our algorithm and measured its performance. The results show that our service is only 3% slower than a standard unreplicated NFS.

### 6. CAP [Brewer’s conjecture and the feasibility of consistent, available, partition-tolerant web services](https://courses.e-ce.uth.gr/CE623/CAP_theorem_proof.pdf) Gilbert S, Lynch N. Acm Sigact News, 2002, 33(2): 51:59.
Abstract: When designing distributed web services, there are three properties that are commonly desired: consistency, availability, and partition tolerance. It is impossible to achieve all three. In this note, we prove this conjecture in the asynchronous network model, and then discuss solutions to this dilemma in the partially synchronous model. 

### 7. BASE [BASE: An Acid Alternative](https://dl.acm.org/citation.cfm?id=1394128).Dan Pritchett.EBay.2008.

Abstract: In partitioned databases, trading some consistency for availability can lead to dramatic improvements in scalability.

### 8. PoW [Bitcoin: A peer-to-peer electronic cash system](http://bitcoins.info/bitcoin.pdf)Nakamoto, Satoshi.2008.
Abstract: A purely peer-to-peer version of electronic cash would allow online payments to be sent directly from one party to another without going through a financial institution. Digital signatures provide part of the solution, but the main benefits are lost if a trusted third party is still required to prevent double-spending. We propose a solution to the double-spending problem using a peer-to-peer network. The network timestamps transactions by hashing them into an ongoing chain of hashbased proof-of-work, forming a record that cannot be changed without redoing the proof-of-work. The longest chain not only serves as proof of the sequence of events witnessed, but proof that it came from the largest pool of CPU power. As long as a majority of CPU power is controlled by nodes that are not cooperating to attack the network, they'll generate the longest chain and outpace attackers. The network itself requires minimal structure. Messages are broadcast on a best effort basis, and nodes can leave and rejoin the network at will, accepting the longest proofof-work chain as proof of what happened while they were gone.

### 9. PoS [Proof of Stake](https://en.bitcoin.it/wiki/Proof).QuantumMechanic.2011.
Abstract: Proof of Stake is a proposed alternative to Proof of Work. Like proof of work, proof of stake attempts to provide consensus and doublespend prevention (see "main" bitcointalk thread, and a Bounty Thread). Because creating forks is costless when you aren't burning an external resource Proof of Stake alone is considered to an unworkable consensus mechanism.

### 10. Ripple [The Ripple Protocol Consensus Algorithm](https://www.cryptiaexchange.com/Whitepaper_Ripple.pdf)
Abstract: While several consensus algorithms exist for the Byzantine Generals Problem, specifically as it pertains to distributed payment systems, many suffer from high latency induced by the requirement that all nodes within the network communicate synchronously. In this work, we present a novel consensus algorithm that circumvents this requirement by utilizing collectively-trusted subnetworks within the larger network. We show that the “trust” required of these subnetworks is in fact minimal and can be further reduced with principled choice of the member nodes. In addition, we show that minimal connectivity is required to maintain agreement throughout the whole network. The result is a low-latency consensus algorithm which still maintains robustness in the face of Byzantine failures. We present this algorithm in its embodiment in the Ripple Protocol.

### 11. DPoS [Delegated Proof of Stake](http://docs.bitshares.org/bitshares/dpos.html).Larimer, Daniel. 2014.

### 12. Raft [In search of an understandable consensus algorithm](https://www.usenix.org/conference/atc14/technical-sessions/presentation/ongaro).Diego Ongaro and John Ousterhout,2014.
Abstract: Raft is a consensus algorithm for managing a replicated log. It produces a result equivalent to (multi-)Paxos, and it is as efficient as Paxos, but its structure is different from Paxos; this makes Raft more understandable than Paxos and also provides a better foundation for building practical systems. In order to enhance understandability, Raft separates the key elements of consensus, such as leader election, log replication, and safety, and it enforces a stronger degree of coherency to reduce the number of states that must be considered. Results from a user study demonstrate that Raft is easier for students to learn than Paxos. Raft also includes a new mechanism for changing the cluster membership, which uses overlapping majorities to guarantee safety.

### 13. PoSV [Proof of stake velocity](https://reddcoin.com/papers/PoSV.pdf)Ren L.April 10, 2018. 
Abstract: Proof of Stake Velocity (PoSV) is proposed as an alternative to Proof of Work (PoW) and Proof of Stake (PoS) to secure the peer-to-peer network and confirm transactions of Reddcoin, a cryptocurrency created specifically to facilitate social interactions in the digital age. PoSV is designed to encourage both ownership (Stake) and activity (Velocity) which directly correspond to the two main functions of Reddcoin as a real currency: store of value and medium of exchange. Reddcoin can also function as the unit of account in heterogeneous social context. The technological aspects of PoSV are presented after a detailed review of existing designs. The economic aspects of Reddcoin are then analysed. Finally the unique position of Reddcoin as a digital social currency in the competitive landscape of cryptocurrencies is discussed.

### 14. Tendermint [The latest gossip on BFT consensus](https://arxiv.org/pdf/1807.04938.pdf)
Abstract: The paper presents Tendermint, a new protocol for ordering events in a distributed network under adversarial conditions. More commonly known as Byzantine Fault Tolerant (BFT) consensus or atomic broadcast, the problem has attracted significant attention in recent years due to the widespread success of blockchain-based digital currencies, such as Bitcoin and Ethereum, which successfully solved the problem in a public setting without a central authority. Tendermint modernizes classic academic work on the subject and simplifies the design of the BFT algorithm by relying on a peer-to-peer gossip protocol among nodes.

### 15.  Ouroboros [Ouroboros: A provably secure proof-of-stake blockchain protocol](https://link.springer.com/chapter/10.1007/978-3-319-63688-7_12) Kiayias, Aggelos. Springer, Cham, 2017.
Abstract:We present “Ouroboros”, the first blockchain protocol based on proof of stake with rigorous security guarantees. We establish security properties for the protocol comparable to those achieved by the bitcoin blockchain protocol. As the protocol provides a “proof of stake” blockchain discipline, it offers qualitative efficiency advantages over blockchains based on proof of physical resources (e.g., proof of work). We also present a novel reward mechanism for incentivizing Proof of Stake protocols and we prove that, given this mechanism, honest behavior is an approximate Nash equilibrium, thus neutralizing attacks such as selfish mining.

### 16.  HoneyBadgerBFT [The Honey Badger of BFT Protocols](https://dl.acm.org/citation.cfm?id=2978399).Miller A, Xia Y, Croman K, Shi E,Song D. In: Proceedings of the 2016 ACM SIGSAC Conference on Computer and Communications Security. Xi’an, China: ACM, 2016. 
Abstract: The surprising success of cryptocurrencies has led to a surge of interest in deploying large scale, highly robust, Byzantine fault tolerant (BFT) protocols for mission-critical applications, such as financial transactions. Although the conventional wisdom is to build atop a (weakly) synchronous protocol such as PBFT (or a variation thereof), such protocols rely critically on network timing assumptions, and only guarantee liveness when the network behaves as expected. We argue these protocols are ill-suited for this deployment scenario. We present an alternative, HoneyBadgerBFT, the first practical asynchronous BFT protocol, which guarantees liveness without making any timing assumptions. We base our solution on a novel atomic broadcast protocol that achieves optimal asymptotic efficiency. We present an implementation and experimental results to show our system can achieve throughput of tens of thousands of transactions per second, and scales to over a hundred nodes on a wide area network. We even conduct BFT experiments over Tor, without needing to tune any parameters. Unlike the alternatives, HoneyBadgerBFT simply does not care about the underlying network.

### 17.  Bitcoin-NG [Bitcoin-NG: A Scalable Blockchain Protocol](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-eyal.pdf). Ittay Eyal, Adem Efe Gencer, Emin Gün Sirer, and Robbert van Renesse, Cornell University. 2016.
Abstract: Cryptocurrencies, based on and led by Bitcoin, have shown promise as infrastructure for pseudonymous online payments, cheap remittance, trustless digital asset exchange, and smart contracts. However, Bitcoin-derived blockchain protocols have inherent scalability limits that trade off between throughput and latency, which withhold the realization of this potential.
This paper presents Bitcoin-NG (Next Generation), a new blockchain protocol designed to scale. Bitcoin-NG is a Byzantine fault tolerant blockchain protocol that is robust to extreme churn and shares the same trust model as Bitcoin.
In addition to Bitcoin-NG, we introduce several novel metrics of interest in quantifying the security and efficiency of Bitcoin-like blockchain protocols. We implement Bitcoin-NG and perform large-scale experiments at 15% the size of the operational Bitcoin system, using unchanged clients of both protocols. These experiments demonstrate that Bitcoin-NG scales optimally, with bandwidth limited only by the capacity of the individual nodes and latency limited only by the propagation time of the network.

### 18. Tangaroa [Tangaroa: a byzantine fault tolerant
raft](http://www.scs.stanford.edu/14au-cs244b/labs/projects/copeland_zhong.pdf).Christopher Copeland and Hongxia Zhong.2016.
Abstract: We propose a Byzantine Fault Tolerant variant of the Raft consensus algorithm, BFTRaft, inspired by the original Raft[1] algorithm and the Practical Byzantine Fault Tolerance algorithm[2]. BFT Raft maintains the safety, fault tolerance, and liveness properties of Raft in the presence of Byzantine faults, while also aiming towards to Raft’s goal of simplicity and understandability. We have implemented a proof-of-concept of this algorithm in the Haskell programming language.


### 19.  Kadena [Kadena: The flrst scalable, high performance private blockchain](http://kadena.io/docs/Kadena-ConsensusWhitePaperAug2016.pdf)Martino W. Kadena.April 10, 2018.
Abstract: This paper introduces Kadena, the first private/permissioned blockchain technology to achieve high performance at scale. Kadena is an implementation of the novel ScalableBFT consensus protocol, which draws inspiration from the Tangaroa protocol as well as practical engineering realities. Until now, private blockchain technologies have been able to provide either high performance or scalability but not both. Rarely deployed into production, BFT-Consensus algorithms achieve high performance initially, but exhibit drastic performance degradation as cluster size increases. Mining (or “proof of work”) is the only workable alternative: it has practically no scaling limit. However, being a probabilistic mechanism, mining is necessarily slow and thus unable to attain the performance demanded by enterprise use-cases. 
The ability to perform at scale, without sacrificing the guarantees that blockchains provide, has been a major unresolved problem in the implementation of private blockchains. Scaling is critical for industrial adoption. Blockchain applications must be able to maintain acceptable performance for a successful deployment to sustain wide and growing participation.

### 20. Stellar [The stellar consensus protocol: A federated model for internet-level consensus](https://www.stellar.org/papers/stellar-consensus-protocol.pdf)
Abstract: This paper introduces a new model for consensus called federated Byzantine agreement (FBA). FBA achieves robustness through quorum slices—individual trust decisions made by each node that together determine system-level quorums. Slices bind the system together much the way individual networks’ peering and transit decisions now unify the Internet.
We also present the Stellar Consensus Protocol (SCP), a construction for FBA. Like all Byzantine agreement protocols, SCP makes no assumptions about the rational behavior of attackers. Unlike prior Byzantine agreement models, which presuppose a unanimously accepted membership list, SCP enjoys open membership that promotes organic network growth. Compared to decentralized proof of-work and proof-of-stake schemes, SCP has modest computing and financial requirements, lowering the barrier to entry and potentially opening up financial systems to new participants.


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


