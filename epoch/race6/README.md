### Notes
- Reflection on Q1, Need to develope a sense of intuition on what context means in contract<br>
- Reflection on Q7, NatSpec and inlined comments is important<br>
- Look into differences between _mint() and _safeMint() [Ans](https://ethereum.stackexchange.com/questions/115280/mint-vs-safemint-which-is-best-for-erc721)<br>
- New magic with unchecked for loop [Ans](https://ethereum.stackexchange.com/questions/127637/how-to-write-an-unchecked-for-loop)

### Questions
[Q1] The security concern(s) with InSecureumLand is/are<br>
(A): Single-step ownership change<br>
(B): Incorrectly implemented KYC check using Merkle proofs<br>
(C): Missing time-delayed change of critical parameters<br>
(D): Accidentally sent Ether gets locked in contract<br>
[Answers]: A, C


[Q2] The security concern(s) with InSecureumLand setOperator() is/are<br>
(A): Missing zero-address validation<br>
(B): Missing event emission<br>
(C): Incorrect modifier<br>
(D): None of the above<br>
[Answers]: A, B


[Q3] The security concern(s) with InSecureumLand mintLands() is/are<br>
(A): Minting could exceed max supply<br>
(B): Minting could exceed maxMintPerTx<br>
(C): Minting could exceed maxMintPerAddress<br>
(D): None of the above<br>
[Answers]: A


[Q4] Missing threshold check(s) on parameter(s) is/are a concern in<br>
(A): mintLands<br>
(B): startPublicSale<br>
(C): contributorsClaimLand<br>
(D): None of the above<br>
[Answers]: B, C


[Q5] The security concern(s) with InSecureumLand contributors claim functions is/are<br>
(A): Anyone can call startContributorsClaimPeriod<br>
(B): Anyone can call stopContributorsClaimPeriod<br>
(C): Anyone can call contributorsClaimLand<br>
(D): None of the above<br>
[Answers]: C


[Q6] The security concern(s) with InSecureumLand random number usage is/are<br>
(A): It depends on miner-influenceable block.timestamp<br>
(B): It depends on miner-influenceable blockhash<br>
(C): It depends on deprecated Chainlink VRF v1<br>
(D): None of the above<br>
[Answers]: C


[Q7] The documentation/readability concern(s) with InSecureumLand is/are<br>
(A): Stale comments<br>
(B): Missing NatSpec<br>
(C): Minimal inlined comments<br>
(D): None of the above<br>
[Answers]: B, C


[Q8] Potential gas optimization(s) (after appropriate security considerations) in InSecureumLand is/are<br>
(A): Removing nonReentrant modifier if mint addresses are known to be EOA<br>
(B): Using _mint instead of _safeMint if mint addresses are known to be EOA<br>
(C): Using unchecked in for loop increments<br>
(D): None of the above<br>
[Answers]: A, B, C
