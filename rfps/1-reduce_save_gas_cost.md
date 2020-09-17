# General Grant Proposal

* **Project:** Reducing gas costs of SAVE mechanism

## Project Overview

### Overview

Transacting with mStable's SAVE mechanism currently requires a large amount of gas. At high ETH prices, this can result in exorbitantly high transaction fees. In order to cater for smaller deposits and withdrawals, we envisage a "cache" mechanism, whereby the underlying interest-generating protocols are not interacted with unless the size of the transaction breaches a certain threshold.

### Project Details

Where relevant, please include

* Mockups/designs/wireframes
* API/interface definitions
* Architecture documentation

@TODO Alex Scott

## Development Roadmap

### Overview
* **Total Estimated Duration:** 1 week
* **Full-time equivalent (FTE):** 1
* **Total Costs:** $5k

### Milestone 1 - Implement SAVE Cache
* **Estimated Duration:** 1 week
* **FTE:** 1
* **Costs:** $5k

| Number | Deliverable | Specification |
| ------------- | ------------- | ------------- |
| 0a. | License | Apache 2.0 / MIT / Unlicense |
| 0b. | Documentation | We will provide both inline documentation of the code and a report of gas costs for the new mechanism. |
| 0c. | Testing Guide | The code will have 100% unit test coverage to ensure functionality and robustness. In the guide we will describe how to run these tests. |
| 1. | SAVE Cache Mechanism | We will create the cache mechanism which ensures thet deposits/withdrawals do not interact with underlying protocols unless dealing with an amount of mUSD over a certain threshold. |
| 2. | Configurability | Allow configuration of the threshold at which deposits and withdrawals will use the cache. |
| 3. | Configurability | Allow configuration of the target size of the cache as a percentage of the total mUSD in SAVE. |