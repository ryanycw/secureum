### Notes
- Reflection on Q2, Single-step ownership change is an issue
- Q9, Q10 not quite get it

### Questions
[Q1] The mint price of an InSecureumApe is <br>
(A): 0.0008 ETH <br>
(B): 0.008 ETH <br>
(C): 0.08 ETH <br>
(D): 0.8 ETH <br>
[Answers]: D


[Q2] The security concern(s) with InSecureumApe access control is/are <br>
(A): Owner can arbitrarily pause public minting of InSecureumApes <br>
(B): Owner can arbitrarily mint InSecureumApes <br>
(C): Single-step ownership change <br>
(D): Missing event emits in and time-delayed effects of owner functions <br>
[Answers]: A, B, C, D


[Q3] The security concern(s) with InSecureumApe constructor is/are <br>
(A): Missing sanity/threshold check on maxNftSupply <br>
(B): Missing sanity/threshold check on saleStart <br>
(C): Potential integer overflow <br>
(D): None of the above <br>
[Answers]: A, B, C


[Q4] The total number of InSecureumApes that can ever be minted is <br>
(A): maxApePurchase <br>
(B): MAX_APES <br>
(C): MAX_APES + 30 <br>
(D): type(uint256).max <br>
[Answers]: D


[Q5] The public minting of InSecureumApes <br>
(A): Must be paid the exact amount in Ether <br>
(B): May be performed 19 NFTs at a time <br>
(C): Uses _safeMint to prevent locked/stuck NFTs <br>
(D): None of the above <br>
[Answers]: B, C


[Q6] The security concern(s) with InSecureumApe is/are <br>
(A): Use of a floating pragma and an older compiler version <br>
(B): Oracle price manipulation <br>
(C): Reentrancy allowing bypass of maxApePurchase check <br>
(D): None of the above <br>
[Answers]: A, C


[Q7] The starting index determination <br>
(A): Is meant to randomize NFT reveal post-mint <br>
(B): Can be triggered by the owner at any time <br>
(C): May be triggered only 9 days after sale start <br>
(D): Accounts for the fact that EVM only stores previous 256 block hashes <br>
[Answers]: A, B, D


[Q8] Potential gas optimization(s) in InSecureumApe is/are <br>
(A): Caching of storage variables <br>
(B): Avoiding initializations of variables to default values of their types <br>
(C): Use of immutables <br>
(D): None of the above <br>
[Answers]: A, B, C