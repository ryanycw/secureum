### Notes
- Figure out UUPS, Beacon, Transparent, Metamorphic

### Questions
[Q1] The function signature is the first 4 bytes of the keccak hash which <br>
(A): Includes the function name <br>
(B): Includes a comma separated list of parameter types <br>
(C): Includes a comma separated list of return value types <br>
(D): Is generated only for public and external functions <br>
[Answers]: A, B, D


[Q2] The Proxy contract is most similar to a <br>
(A): UUPS Proxy <br>
(B): Beacon Proxy <br>
(C): Transparent Proxy <br>
(D): Metamorphic Proxy <br>
[Answers]: C


[Q3] Gas will be saved with the following changes <br>
(A): Skipping initialization of counter variable <br>
(B): Making increase() function external to avoid copying from calldata to memory <br>
(C): Packing multiple implementation addresses into the same storage slot <br>
(D): Moving the calculation of the counter() function's signature hash to a constant <br>
[Answers]: A


[Q4] Calling the increase() function on the Proxy contract <br>
(A): Will revert since the Proxy contract has no increase() function <br>
(B): Will revert for any other caller than the one that deployed the Proxy <br>
(C): Increases the integer value in the Proxy's storage slot located at index 1 <br>
(D): Delegate-calls to the zero-address <br>
[Answers]: B, C


[Q5] Calling the decrease() function on the Proxy contract <br>
(A): Will revert because it was not correctly registered on the proxy <br>
(B): Will succeed and return the value of counter after it was decreased <br>
(C): Will succeed and return the value of counter before it was decreased <br>
(D): Will succeed and return nothing <br>
[Answers]: D


[Q6] Due to a storage clash between the Proxy and the Mastercopy contracts <br>
(A): Proxy's implementations would be overwritten by 0 during initialization of the Mastercopy <br>
(B): Proxy's implementations would be overwritten when the counter variable changes <br>
(C): Proxy's implementations variable's storage slot being overwritten causes a DoS <br>
(D): None of the above <br>
[Answers]: D


[Q7] The Proxy contract <br>
(A): Won't be able to receive any ether when calldatasize is 0 due to a missing receive() <br>
(B): Will be the owner of the Mastercopy contract <br>
(C): Has a storage clash in slot 0 which will cause issues with the current Mastercopy <br>
(D): None of the above <br>
[Answers]: B


[Q8] The fallback() function's assembly block <br>
(A): Can be marked as "memory-safe" for gas optimizations <br>
(B): Has the result of the delegate-call overwrite the the call parameters in memory <br>
(C): Interferes with the Slot-Hash calculation for the implementations-mapping by overwriting the scratch space <br>
(D): None of the above <br>
[Answers]: B