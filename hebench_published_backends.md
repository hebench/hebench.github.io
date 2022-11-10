# Available Backends

- [HEBench Home](https://hebench.org/)
- [About HEBench](https://hebench.org/faq#what-is-hebench)
- Available Backends
  - [Reference Backends](#reference-backends)
  - [Third-Party Backends](#third-party-backends)
- [Getting Started](https://hebench.org/documentation/getting-started)
- [Governance](https://hebench.org/about/governance)
- [Code of Conduct](https://hebench.org/about/code-of-conduct)

<br>

## Reference Backends

The HEBench Reference Backends are shared libraries that implement the required functions specified in either the hebench::APIBridge or hebench::cpp wrapper. They are intended only as a reference on how to implement a backend for HEBench using a particular library. **_None of these libraries are fully optimized for performance._**

  Repository   | Latest Update | Versions | Description
-------------- | ------------ | ------------ | ------------
[Cleartext Backend](https://github.com/hebench/backend-cpu-cleartext) | Oct 20, 2022 | *Backend*: v0.7.0-beta <br /> *API Bridge*: v0.7.1-beta <br /> N/A | Clear text backend which implements all tests without encryption.
[HElib Backend](https://github.com/hebench/reference-helib-backend) |  Nov 07, 2022 | *Backend*: v0.1.0-beta <br /> *API Bridge*: v0.7.0-beta <br /> *HElib*: v2.2.1  | Backend which uses HElib homomorphic encryption library to perform tests on encrypted data.
[PALISADE Backend](https://github.com/hebench/reference-palisade-backend) |  Aug 25, 2022 | *Backend*: v0.7.0-beta <br /> *API Bridge*: v0.7.0-beta <br /> *PALISADE*: v1.11.6  | Backend which uses PALISADE lattice encryption library to perform tests on encrypted data.
[SEAL Backend](https://github.com/hebench/reference-seal-backend)     | Aug 25, 2022 | *Backend*: v0.7.0-beta <br /> *API Bridge*: v0.7.0-beta <br /> *SEAL*: v3.7.2  | Backend which uses Microsoft SEAL library to perform tests on encrypted data.

## Third-Party Backends

Repository | Description
-------------- | ------------
N/A | N/A

<br/>

Back to [HEBench Home](https://hebench.org/)
