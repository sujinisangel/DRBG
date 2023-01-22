# DRBG (NIST SP800-90A)
## DRBG Mechanism
### Instantiating
#### <Input>
Instantiate_function(requested_instantiation_security_strength, prediction_resistance_flag, personalization_string)
#### <Output>
status, state_handle
#### <Process>
1. Checks the  validity of the input parameters
2. Determines the security strength for the DRBG instantiation
3. Obtains entropy input with entropy sufficient to support the security strength
4. Obtains the nonce (if required)
5. Determines the initial internal state using the instantiate algorith
6. If an implementation supports multiple simultaneous instantiations of the same DRBG
- Reseeding
- Generating
- Uninstantiating
