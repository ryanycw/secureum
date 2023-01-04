### Notes
- Array lengths check
- Underflow/overflow will happen in "unchecked" after 0.8.0
- In Q5, why event emission is incorrect?

### Questions
[Q1] InSecureum balanceOf()<br>
(A): May be optimised by caching state variable in local variable<br>
(B): May be optimised by changing state mutability from view to pure<br>
(C): May be optimised by changing its visibility to external<br>
(D): None of the above<br>
[Answers]: D


[Q2] In InSecureum, array lengths mismatch check is missing in<br>
(A): balanceOfBatch()<br>
(B): _safeBatchTransferFrom()<br>
(C): _mintBatch()<br>
(D): _burnBatch()<br>
[Answers]: A, B, C, D


[Q3] The security concern(s) with InSecureum _safeTransferFrom() is/are<br>
(A): Incorrect visibility<br>
(B): Susceptibility to an integer underflow<br>
(C): Missing zero-address validation<br>
(D): None of the above<br>
[Answers]: A, B, C


[Q4] The security concern(s) with InSecureum _safeBatchTransferFrom() is/are<br>
(A): Missing array lengths mismatch check<br>
(B): Susceptibility to an integer underflow<br>
(C): Incorrect balance update<br>
(D): None of the above<br>
[Answers]: A, C


[Q5] The security concern(s) with InSecureum _mintBatch() is/are<br>
(A): Missing array lengths mismatch check<br>
(B): Incorrect event emission<br>
(C): Allows burning of tokens<br>
(D): None of the above<br>
[Answers]: A, B, C


[Q6] The security concern(s) with InSecureum _burn() is/are<br>
(A): Missing zero-address validation<br>
(B): Susceptibility to an integer underflow<br>
(C): Incorrect balance update<br>
(D): None of the above<br>
[Answers]: D


[Q7] The security concern(s) with InSecureum _doSafeTransferAcceptanceCheck() is/are<br>
(A): isContract check on incorrect address<br>
(B): Incorrect check on return value<br>
(C): Call to incorrect isContract implementation<br>
(D): None of the above<br>
[Answers]: B, C


[Q8] The security concern(s) with InSecureum isContract() implementation is/are<br>
(A): Incorrect visibility<br>
(B): Incorrect operator in the comparison<br>
(C): Unnecessary because Ethereum only has Contract accounts<br>
(D): None of the above<br>
[Answers]: B
