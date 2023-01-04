### Notes
What is "unchecked" for? [Ans](https://ethereum.stackexchange.com/questions/113221/what-is-the-purpose-of-unchecked-in-solidity)<br>
What is "pure state mutability"? <br> [Ans](https://medium.com/coinmonks/function-state-mutability-in-solidity-acb850eedccc)
Why is Q4A, Q5B incorrect? <br> [Ans](https://hackernoon.com/hack-solidity-integer-overflow-and-underflow)


### Questions
[Q1] InSecureum implements<br>
(A): Atypical decimals value<br>
(B): Non-standard decreaseAllowance and increaseAllowance<br>
(C): Non-standard transfer<br>
(D): None of the above<br>
[Answers]: A, B


[Q2] In InSecureum<br>
(A): decimals() can have pure state mutability instead of view<br>
(B): _burn() can have external visibility instead of internal<br>
(C): _mint() should have internal visibility instead of external<br>
(D): None of the above<br>
[Answers]: A, C


[Q3] InSecureum transferFrom()<br>
(A): Is susceptible to an integer underflow<br>
(B): Has an incorrect allowance check<br>
(C): Has an optimisation indicative of unlimited approvals<br>
(D): None of the above<br>
[Answers]: A, B, C


[Q4] In InSecureum<br>
(A): increaseAllowance is susceptible to an integer overflow<br>
(B): decreaseAllowance is susceptible to an integer overflow<br>
(C): decreaseAllowance does not allow reducing allowance to zero<br>
(D): decreaseAllowance can be optimised with unchecked{}<br>
[Answers]: C, D


[Q5] InSecureum _transfer()<br>
(A): Is missing a zero-address validation<br>
(B): Is susceptible to an integer overflow<br>
(C): Is susceptible to an integer underflow<br>
(D): None of the above<br>
[Answers]: D


[Q6] InSecureum _mint()<br>
(A): Is missing a zero-address validation<br>
(B): Has an incorrect event emission<br>
(C): Has an incorrect update of account balance<br>
(D): None of the above<br>
[Answers]: A, C


[Q7] InSecureum _burn()<br>
(A): Is missing a zero-address validation<br>
(B): Has an incorrect event emission<br>
(C): Has an incorrect update of account balance<br>
(D): None of the above<br>
[Answers]: B


[Q8] InSecureum _approve()<br>
(A): Is missing a zero-address validation<br>
(B): Has incorrect error messages<br>
(C): Has an incorrect update of allowance<br>
(D): None of the above<br>
[Answers]: B, C