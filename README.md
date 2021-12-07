# HEBench Home

Project name: **HE Benchmarking Framework - HEBench**

- [What is HEBench](#what-is-hebench)
  - [What is Homomorphic Encryption](#what-is-homomorphic-encryption)
- [What Does HEBench Offer](#what-does-hebench-offer)
- [Software Components and Architecture](#software-components-and-architecture)
- [What Can Be Done with HEBench](#what-can-be-done-with-hebench)
- [Available Backends](hebench_published_backends.md)
- [Getting Started](quickstart_guide.md)
- [HEBench Governance](governance.md)

## What is HEBench
A flexible benchmarking framework for Homomorphic Encryption that allows fair performance comparison among different implementations (in hardware and/or software) of a collection of homomorphic encryption workloads.

HEBench project is hosted at [https://github.com/hebench](https://github.com/hebench) .

### What is Homomorphic Encryption
Homomorphic Encryption (HE) refers to a form of encryption which enables computation in the encrypted domain without requiring access to a private key. This technology enables unprecedented capabilities for secure outsourced computation.

More information can be found at [Homomorphic Encryption Standardization](https://homomorphicencryption.org/introduction).

## What Does HEBench Offer
The main objective of HEBench is to allow users to create backends that implement their solutions to a set of supported workloads to be benchmarked by HEBench's Test Harness. To this end, HEBench offers a flexible C API that enables implementation of such backends to test HE APIs, algorithms, optimizations, hardware, etc.

A backend is a shared library that exposes its functionality through the API Bridge interface, compatible with the Test Harness. A backend can focus on specific workloads to benchmark; it does not need to implement every possible workload supported by Test Harness.

With this release, some reference backends have been published as well. As reference, they show how users might implement their own backends to fit their needs.

## Software Components and Architecture
![Graphical representation of software components and architecture](https://github.com/hebench/frontend/blob/main/docsrc/images/architecture.png?raw=true)

**Test Harness** and **backend Loader** (w/ extensible workload framework): Main frontend component that drives the benchmarking of the workload operations.

Currently supported categories:

* Latency: measures end-to-end latency (time to complete) for a single operation
* Offline: measures throughput (ops/sec) that a backend can perform on a batch of data.

Currently supported workloads:

* Element-wise vector addition
* Element-wise vector multiplication
* Vector dot product
* Matrix multiplication
* Logistic regression inference

The dynamic backend loader allows the Test Harness to dynamically link to any backend that implements the API Bridge interface.

**API Bridge with C++ Wrapper** (w/ documentation and example): API Bridge offers a uniform C interface that bridges the communication between Test Harness and backends. Test Harness communicates and issues commands to backends for the operations to perform via the API Bridge. Operations and their results are validated and timed by Test Harness.

C++ wrapper is a thin wrapper around the API Bridge. It offers a utility library that encapsulates common functionality expected by the API Bridge and hides boilerplate code, easing the development of backends by users.

A backend example is shipped with the frontend that contains a simple implementation of a workload in clear-text. This is intended to be used as a starting point for any new backends.

**Clear text backend reference (CPU)**: A reference backend that performs the operations of all supported workloads in clear text. This is intended as an extended reference on how to implement a fully functional backend, and as a unit test for the Test Harness.

**SEAL backend reference (CPU)**: A reference backend that performs the operations of some of the supported workloads. This is intended as a reference to an actual implementation of the workloads in the HE space. It uses Microsoft SEAL library for the HE operations.

**PALISADE backend reference (CPU)**: A reference backend that performs the operations of some of the supported workloads. This is intended as a reference to an actual implementation of the workloads in the HE space. It uses PALISADE lattice cryptography library for the HE operations.

## What Can Be Done with HEBench
Out of the box, users can run the benchmark from the API Bridge example, clear text, reference SEAL, and reference PALISADE backends. These run on CPU using the specified API support.

Flexibility to create new backends is already in place and users are encouraged to create their own to benchmark their HE implementations in whichever hardware or system it may be hosted.

Users can benchmark their own implementations with HEBench (by creating their own backends) and compare results with other implementations of published backends. The framework is designed to give a fair shot to all users to put their best foot forward when implementing their solutions.

## Available backends

For a list of available backends, visit [Published Backends](hebench_published_backends.md).

## Getting Started

Check out the [HEBench Quick Start Guide](quickstart_guide.md) to get started with running  benchmarks.

Find the complete reference to HEBench in the [Documentation](https://hebench.github.io/frontend).

## HEBench Governance
Policies and procedures that manage the HEBench project and community can be found in the [Governance document](governance.md).

