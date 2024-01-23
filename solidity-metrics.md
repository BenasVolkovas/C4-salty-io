[<img width="200" alt="get in touch with Consensys Diligence" src="https://user-images.githubusercontent.com/2865694/56826101-91dcf380-685b-11e9-937c-af49c2510aa0.png">](https://diligence.consensys.net)<br/>
<sup>
[[ 🌐 ](https://diligence.consensys.net) [ 📩 ](mailto:diligence@consensys.net) [ 🔥 ](https://consensys.github.io/diligence/)]
</sup><br/><br/>

# Solidity Metrics for 'CLI'

## Table of contents

- [Solidity Metrics for 'CLI'](#solidity-metrics-for-cli)
  - [Table of contents](#table-of-contents)
  - [Scope](#scope)
    - [Source Units in Scope](#source-units-in-scope)
      - [Out of Scope](#out-of-scope)
        - [Excluded Source Units](#excluded-source-units)
        - [Duplicate Source Units](#duplicate-source-units)
        - [Doppelganger Contracts](#doppelganger-contracts)
  - [Report](#report)
    - [Overview](#overview)
      - [Risk](#risk)
      - [Source Lines (sloc vs. nsloc)](#source-lines-sloc-vs-nsloc)
      - [Inline Documentation](#inline-documentation)
      - [Components](#components)
      - [Exposed Functions](#exposed-functions)
      - [StateVariables](#statevariables)
      - [Capabilities](#capabilities)
      - [Dependencies / External Imports](#dependencies--external-imports)
      - [Totals](#totals)
        - [Summary](#summary)
        - [AST Node Statistics](#ast-node-statistics)
          - [Function Calls](#function-calls)
          - [Assembly Calls](#assembly-calls)
          - [AST Total](#ast-total)
        - [Inheritance Graph](#inheritance-graph)
        - [CallGraph](#callgraph)
          - [Contract Summary](#contract-summary)

## <span id=t-scope>Scope</span>

This section lists files that are in scope for the metrics report.

-   **Project:** `'CLI'`
-   **Included Files:**
    -   ``
-   **Excluded Paths:**
    -   ``
-   **File Limit:** `undefined`

    -   **Exclude File list Limit:** `undefined`

-   **Workspace Repository:** `unknown` (`undefined`@`undefined`)

### <span id=t-source-Units-in-Scope>Source Units in Scope</span>

Source Units Analyzed: **`35`**<br>
Source Units in Scope: **`35`** (**100%**)

| Type   | File                                  | Logic Contracts | Interfaces | Lines    | nLines   | nSLOC    | Comment Lines | Complex. Score | Capabilities                                                                                                                                                                                                                                                    |
| ------ | ------------------------------------- | --------------- | ---------- | -------- | -------- | -------- | ------------- | -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎨     | src/arbitrage/ArbitrageSearch.sol     | 1               | \*\*\*\*   | 137      | 134      | 69       | 38            | 44             | **<abbr title='Unchecked Blocks'>Σ</abbr>**                                                                                                                                                                                                                     |
| 📝     | src/dao/DAO.sol                       | 1               | \*\*\*\*   | 388      | 376      | 239      | 47            | 237            | **<abbr title='Uses Hash-Functions'>🧮</abbr>**                                                                                                                                                                                                                 |
| 📝     | src/dao/DAOConfig.sol                 | 1               | \*\*\*\*   | 198      | 190      | 126      | 35            | 69             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/dao/Proposals.sol                 | 1               | \*\*\*\*   | 446      | 421      | 242      | 63            | 243            | **<abbr title='Uses Hash-Functions'>🧮</abbr>**                                                                                                                                                                                                                 |
| 🎨     | src/dao/Parameters.sol                | 1               | \*\*\*\*   | 123      | 122      | 92       | 14            | 53             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/launch/Airdrop.sol                | 1               | \*\*\*\*   | 101      | 96       | 51       | 17            | 49             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/launch/BootstrapBallot.sol        | 1               | \*\*\*\*   | 86       | 84       | 49       | 11            | 36             | **<abbr title='Uses Hash-Functions'>🧮</abbr>**                                                                                                                                                                                                                 |
| 📝     | src/launch/InitialDistribution.sol    | 1               | \*\*\*\*   | 75       | 74       | 50       | 8             | 34             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📚     | src/pools/PoolUtils.sol               | 1               | \*\*\*\*   | 69       | 66       | 30       | 18            | 35             | **<abbr title='Uses Hash-Functions'>🧮</abbr>**                                                                                                                                                                                                                 |
| 📝     | src/pools/PoolsConfig.sol             | 1               | \*\*\*\*   | 156      | 147      | 87       | 20            | 69             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 🎨     | src/pools/PoolStats.sol               | 1               | \*\*\*\*   | 147      | 140      | 82       | 21            | 73             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/pools/Pools.sol                   | 1               | \*\*\*\*   | 427      | 410      | 212      | 94            | 147            | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📚     | src/pools/PoolMath.sol                | 1               | \*\*\*\*   | 228      | 224      | 65       | 131           | 29             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/price_feed/CoreChainlinkFeed.sol  | 1               | \*\*\*\*   | 73       | 70       | 44       | 14            | 20             | **<abbr title='TryCatch Blocks'>♻️</abbr>**                                                                                                                                                                                                                     |
| 📝     | src/price_feed/CoreUniswapFeed.sol    | 1               | \*\*\*\*   | 145      | 139      | 81       | 23            | 67             | **<abbr title='TryCatch Blocks'>♻️</abbr>**                                                                                                                                                                                                                     |
| 📝     | src/price_feed/PriceAggregator.sol    | 1               | \*\*\*\*   | 197      | 187      | 123      | 23            | 68             | **<abbr title='TryCatch Blocks'>♻️</abbr>**                                                                                                                                                                                                                     |
| 📝     | src/price_feed/CoreSaltyFeed.sol      | 1               | \*\*\*\*   | 54       | 52       | 32       | 6             | 18             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/rewards/RewardsConfig.sol         | 1               | \*\*\*\*   | 101      | 97       | 66       | 15            | 37             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/rewards/Emissions.sol             | 1               | \*\*\*\*   | 62       | 61       | 34       | 11            | 22             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/rewards/RewardsEmitter.sol        | 1               | \*\*\*\*   | 151      | 148      | 87       | 29            | 89             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/rewards/SaltRewards.sol           | 1               | \*\*\*\*   | 149      | 143      | 82       | 25            | 110            | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/stable/USDS.sol                   | 1               | \*\*\*\*   | 61       | 58       | 30       | 10            | 27             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/stable/StableConfig.sol           | 1               | \*\*\*\*   | 153      | 147      | 98       | 20            | 53             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/stable/CollateralAndLiquidity.sol | 1               | \*\*\*\*   | 352      | 338      | 176      | 71            | 183            | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/stable/Liquidizer.sol             | 1               | \*\*\*\*   | 153      | 148      | 88       | 28            | 73             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/staking/StakingConfig.sol         | 1               | \*\*\*\*   | 100      | 96       | 66       | 12            | 37             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 🎨     | src/staking/Liquidity.sol             | 1               | \*\*\*\*   | 163      | 158      | 80       | 37            | 68             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 🎨     | src/staking/StakingRewards.sol        | 1               | \*\*\*\*   | 306      | 294      | 157      | 62            | 170            | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/staking/Staking.sol               | 1               | \*\*\*\*   | 213      | 202      | 106      | 37            | 106            | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝     | src/ManagedWallet.sol                 | 1               | \*\*\*\*   | 90       | 88       | 46       | 20            | 36             | **<abbr title='Payable Functions'>💰</abbr>**                                                                                                                                                                                                                   |
| 📝     | src/AccessManager.sol                 | 1               | \*\*\*\*   | 79       | 75       | 31       | 21            | 20             | **<abbr title='Uses Hash-Functions'>🧮</abbr>**                                                                                                                                                                                                                 |
| 📝     | src/Salt.sol                          | 1               | \*\*\*\*   | 40       | 38       | 22       | 4             | 19             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📚     | src/SigningTools.sol                  | 1               | \*\*\*\*   | 30       | 29       | 19       | 2             | 24             | **<abbr title='Uses Assembly'>🖥</abbr><abbr title='Handles Signatures: ecrecover'>🔖</abbr>**                                                                                                                                                                   |
| 📝     | src/Upkeep.sol                        | 1               | \*\*\*\*   | 291      | 277      | 155      | 48            | 151            | **<abbr title='TryCatch Blocks'>♻️</abbr>**                                                                                                                                                                                                                     |
| 📝     | src/ExchangeConfig.sol                | 1               | \*\*\*\*   | 86       | 83       | 55       | 15            | 38             | \*\*\*\*                                                                                                                                                                                                                                                        |
| 📝📚🎨 | **Totals**                            | **35**          | \*\*\*\*   | **5630** | **5412** | **3072** | **1050**      | **2554**       | **<abbr title='Uses Assembly'>🖥</abbr><abbr title='Payable Functions'>💰</abbr><abbr title='Uses Hash-Functions'>🧮</abbr><abbr title='Handles Signatures: ecrecover'>🔖</abbr><abbr title='TryCatch Blocks'>♻️</abbr><abbr title='Unchecked Blocks'>Σ</abbr>** |

<sub>
Legend: <a onclick="toggleVisibility('table-legend', this)">[➕]</a>
<div id="table-legend" style="display:none">

<ul>
<li> <b>Lines</b>: total lines of the source unit </li>
<li> <b>nLines</b>: normalized lines of the source unit (e.g. normalizes functions spanning multiple lines) </li>
<li> <b>nSLOC</b>: normalized source lines of code (only source-code lines; no comments, no blank lines) </li>
<li> <b>Comment Lines</b>: lines containing single or block comments </li>
<li> <b>Complexity Score</b>: a custom complexity score derived from code statements that are known to introduce code complexity (branches, loops, calls, external interfaces, ...) </li>
</ul>

</div>
</sub>

#### <span id=t-out-of-scope>Out of Scope</span>

##### <span id=t-out-of-scope-excluded-source-units>Excluded Source Units</span>

Source Units Excluded: **`0`**

<a onclick="toggleVisibility('excluded-files', this)">[➕]</a>

<div id="excluded-files" style="display:none">
| File   |
| ------ |
| None |

</div>

##### <span id=t-out-of-scope-duplicate-source-units>Duplicate Source Units</span>

Duplicate Source Units Excluded: **`0`**

<a onclick="toggleVisibility('duplicate-files', this)">[➕]</a>

<div id="duplicate-files" style="display:none">
| File   |
| ------ |
| None |

</div>

##### <span id=t-out-of-scope-doppelganger-contracts>Doppelganger Contracts</span>

Doppelganger Contracts: **`0`**

<a onclick="toggleVisibility('doppelganger-contracts', this)">[➕]</a>

<div id="doppelganger-contracts" style="display:none">
| File   | Contract | Doppelganger | 
| ------ | -------- | ------------ |

</div>

## <span id=t-report>Report</span>

### Overview

The analysis finished with **`0`** errors and **`0`** duplicate files.

#### <span id=t-risk>Risk</span>

<div class="wrapper" style="max-width: 512px; margin: auto">
			<canvas id="chart-risk-summary"></canvas>
</div>

#### <span id=t-source-lines>Source Lines (sloc vs. nsloc)</span>

<div class="wrapper" style="max-width: 512px; margin: auto">
    <canvas id="chart-nsloc-total"></canvas>
</div>

#### <span id=t-inline-documentation>Inline Documentation</span>

-   **Comment-to-Source Ratio:** On average there are`3.13` code lines per comment (lower=better).
-   **ToDo's:** `0`

#### <span id=t-components>Components</span>

| 📝Contracts | 📚Libraries | 🔍Interfaces | 🎨Abstract |
| ----------- | ----------- | ------------ | ---------- |
| 27          | 3           | 0            | 5          |

#### <span id=t-exposed-functions>Exposed Functions</span>

This section lists functions that are explicitly declared public or payable. Please note that getter methods for public stateVars are not included.

| 🌐Public | 💰Payable |
| -------- | --------- |
| 174      | 1         |

| External | Internal | Private | Pure | View |
| -------- | -------- | ------- | ---- | ---- |
| 131      | 205      | 0       | 11   | 72   |

#### <span id=t-statevariables>StateVariables</span>

| Total | 🌐Public |
| ----- | -------- |
| 217   | 196      |

#### <span id=t-capabilities>Capabilities</span>

| Solidity Versions observed | 🧪 Experimental Features | 💰 Can Receive Funds | 🖥 Uses Assembly           | 💣 Has Destroyable Contracts |
| -------------------------- | ------------------------ | -------------------- | ------------------------- | ---------------------------- |
| `=0.8.22`                  |                          | `yes`                | `yes` <br/>(1 asm blocks) | \*\*\*\*                     |

| 📤 Transfers ETH | ⚡ Low-Level Calls | 👥 DelegateCall | 🧮 Uses Hash Functions | 🔖 ECRecover | 🌀 New/Create/Create2 |
| ---------------- | ------------------ | --------------- | ---------------------- | ------------ | --------------------- |
| \*\*\*\*         | \*\*\*\*           | \*\*\*\*        | `yes`                  | `yes`        | \*\*\*\*              |

| ♻️ TryCatch | Σ Unchecked |
| ----------- | ----------- |
| `yes`       | `yes`       |

#### <span id=t-package-imports>Dependencies / External Imports</span>

| Dependency / Import Path                                                   | Count |
| -------------------------------------------------------------------------- | ----- |
| chainlink/contracts/src/v0.8/interfaces/AggregatorV3Interface.sol          | 1     |
| openzeppelin-contracts/contracts/access/Ownable.sol                        | 10    |
| openzeppelin-contracts/contracts/finance/VestingWallet.sol                 | 2     |
| openzeppelin-contracts/contracts/security/ReentrancyGuard.sol              | 8     |
| openzeppelin-contracts/contracts/token/ERC20/ERC20.sol                     | 7     |
| openzeppelin-contracts/contracts/token/ERC20/IERC20.sol                    | 4     |
| openzeppelin-contracts/contracts/token/ERC20/extensions/IERC20Metadata.sol | 1     |
| openzeppelin-contracts/contracts/token/ERC20/utils/SafeERC20.sol           | 12    |
| openzeppelin-contracts/contracts/utils/Strings.sol                         | 1     |
| openzeppelin-contracts/contracts/utils/math/Math.sol                       | 4     |
| openzeppelin-contracts/contracts/utils/structs/EnumerableSet.sol           | 4     |
| v3-core/interfaces/IUniswapV3Pool.sol                                      | 1     |
| v3-core/libraries/FixedPoint96.sol                                         | 1     |
| v3-core/libraries/FullMath.sol                                             | 1     |
| v3-core/libraries/TickMath.sol                                             | 1     |

#### <span id=t-totals>Totals</span>

##### Summary

<div class="wrapper" style="max-width: 90%; margin: auto">
    <canvas id="chart-num-bar"></canvas>
</div>

##### AST Node Statistics

###### Function Calls

<div class="wrapper" style="max-width: 90%; margin: auto">
    <canvas id="chart-num-bar-ast-funccalls"></canvas>
</div>

###### Assembly Calls

<div class="wrapper" style="max-width: 90%; margin: auto">
    <canvas id="chart-num-bar-ast-asmcalls"></canvas>
</div>

###### AST Total

<div class="wrapper" style="max-width: 90%; margin: auto">
    <canvas id="chart-num-bar-ast"></canvas>
</div>

##### Inheritance Graph

<a onclick="toggleVisibility('surya-inherit', this)">[➕]</a>

<div id="surya-inherit" style="display:none">
<div class="wrapper" style="max-width: 512px; margin: auto">
    <div id="surya-inheritance" style="text-align: center;"></div> 
</div>
</div>

##### CallGraph

<a onclick="toggleVisibility('surya-call', this)">[➕]</a>

<div id="surya-call" style="display:none">
<div class="wrapper" style="max-width: 512px; margin: auto">
    <div id="surya-callgraph" style="text-align: center;"></div>
</div>
</div>

###### Contract Summary

<a onclick="toggleVisibility('surya-mdreport', this)">[➕]</a>

<div id="surya-mdreport" style="display:none">
 Sūrya's Description Report

Files Description Table

| File Name                             | SHA-1 Hash       |
| ------------------------------------- | ---------------- |
| src/arbitrage/ArbitrageSearch.sol     | [object Promise] |
| src/dao/DAO.sol                       | [object Promise] |
| src/dao/DAOConfig.sol                 | [object Promise] |
| src/dao/Proposals.sol                 | [object Promise] |
| src/dao/Parameters.sol                | [object Promise] |
| src/launch/Airdrop.sol                | [object Promise] |
| src/launch/BootstrapBallot.sol        | [object Promise] |
| src/launch/InitialDistribution.sol    | [object Promise] |
| src/pools/PoolUtils.sol               | [object Promise] |
| src/pools/PoolsConfig.sol             | [object Promise] |
| src/pools/PoolStats.sol               | [object Promise] |
| src/pools/Pools.sol                   | [object Promise] |
| src/pools/PoolMath.sol                | [object Promise] |
| src/price_feed/CoreChainlinkFeed.sol  | [object Promise] |
| src/price_feed/CoreUniswapFeed.sol    | [object Promise] |
| src/price_feed/PriceAggregator.sol    | [object Promise] |
| src/price_feed/CoreSaltyFeed.sol      | [object Promise] |
| src/rewards/RewardsConfig.sol         | [object Promise] |
| src/rewards/Emissions.sol             | [object Promise] |
| src/rewards/RewardsEmitter.sol        | [object Promise] |
| src/rewards/SaltRewards.sol           | [object Promise] |
| src/stable/USDS.sol                   | [object Promise] |
| src/stable/StableConfig.sol           | [object Promise] |
| src/stable/CollateralAndLiquidity.sol | [object Promise] |
| src/stable/Liquidizer.sol             | [object Promise] |
| src/staking/StakingConfig.sol         | [object Promise] |
| src/staking/Liquidity.sol             | [object Promise] |
| src/staking/StakingRewards.sol        | [object Promise] |
| src/staking/Staking.sol               | [object Promise] |
| src/ManagedWallet.sol                 | [object Promise] |
| src/AccessManager.sol                 | [object Promise] |
| src/Salt.sol                          | [object Promise] |
| src/SigningTools.sol                  | [object Promise] |
| src/Upkeep.sol                        | [object Promise] |
| src/ExchangeConfig.sol                | [object Promise] |

Contracts Description Table

|          Contract          |                       Type                       |                            Bases                             |                |                               |
| :------------------------: | :----------------------------------------------: | :----------------------------------------------------------: | :------------: | :---------------------------: |
|             └              |                **Function Name**                 |                        **Visibility**                        | **Mutability** |         **Modifiers**         |
|                            |                                                  |                                                              |                |                               |
|    **ArbitrageSearch**     |                  Implementation                  |                                                              |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                 \_arbitragePath                  |                         Internal 🔒                          |                |                               |
|             └              |              \_rightMoreProfitable               |                         Internal 🔒                          |                |                               |
|             └              |                \_bisectionSearch                 |                         Internal 🔒                          |                |                               |
|                            |                                                  |                                                              |                |                               |
|          **DAO**           |                  Implementation                  |              IDAO, Parameters, ReentrancyGuard               |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |            \_finalizeParameterBallot             |                         Internal 🔒                          |       🛑       |                               |
|             └              |               \_executeSetContract               |                         Internal 🔒                          |       🛑       |                               |
|             └              |              \_executeSetWebsiteURL              |                         Internal 🔒                          |       🛑       |                               |
|             └              |                \_executeApproval                 |                         Internal 🔒                          |       🛑       |                               |
|             └              |             \_finalizeApprovalBallot             |                         Internal 🔒                          |       🛑       |                               |
|             └              |           \_finalizeTokenWhitelisting            |                         Internal 🔒                          |       🛑       |                               |
|             └              |                  finalizeBallot                  |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |             withdrawArbitrageProfits             |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                     formPOL                      |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |              processRewardsFromPOL               |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                   withdrawPOL                    |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                countryIsExcluded                 |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|       **DAOConfig**        |                  Implementation                  |                     IDAOConfig, Ownable                      |                |                               |
|             └              |            changeBootstrappingRewards            |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |          changePercentPolRewardsBurned           |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |          changeBaseBallotQuorumPercent           |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |               changeBallotDuration               |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |        changeRequiredProposalPercentStake        |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |      changeMaxPendingTokensForWhitelisting       |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |         changeArbitrageProfitsPercentPOL         |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |            changeUpkeepRewardPercent             |                         External ❗️                         |       🛑       |           onlyOwner           |
|                            |                                                  |                                                              |                |                               |
|       **Proposals**        |                  Implementation                  |                 IProposals, ReentrancyGuard                  |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |             \_possiblyCreateProposal             |                         Internal 🔒                          |       🛑       |                               |
|             └              |            createConfirmationProposal            |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |              markBallotAsFinalized               |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |              proposeParameterBallot              |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |             proposeTokenWhitelisting             |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |            proposeTokenUnwhitelisting            |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                 proposeSendSALT                  |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |               proposeCallContract                |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |             proposeCountryInclusion              |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |             proposeCountryExclusion              |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |            proposeSetContractAddress             |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |               proposeWebsiteUpdate               |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                     castVote                     |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                   ballotForID                    |                         External ❗️                         |                |             NO❗️             |
|             └              |              lastUserVoteForBallot               |                         External ❗️                         |                |             NO❗️             |
|             └              |                votesCastForBallot                |                         External ❗️                         |                |             NO❗️             |
|             └              |           requiredQuorumForBallotType            |                          Public ❗️                          |                |             NO❗️             |
|             └              |             totalVotesCastForBallot              |                          Public ❗️                          |                |             NO❗️             |
|             └              |                 ballotIsApproved                 |                         External ❗️                         |                |             NO❗️             |
|             └              |               winningParameterVote               |                         External ❗️                         |                |             NO❗️             |
|             └              |                canFinalizeBallot                 |                         External ❗️                         |                |             NO❗️             |
|             └              |                   openBallots                    |                         External ❗️                         |                |             NO❗️             |
|             └              |         openBallotsForTokenWhitelisting          |                         External ❗️                         |                |             NO❗️             |
|             └              |     tokenWhitelistingBallotWithTheMostVotes      |                         External ❗️                         |                |             NO❗️             |
|             └              |              userHasActiveProposal               |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|       **Parameters**       |                  Implementation                  |                                                              |                |                               |
|             └              |             \_executeParameterChange             |                         Internal 🔒                          |       🛑       |                               |
|                            |                                                  |                                                              |                |                               |
|        **Airdrop**         |                  Implementation                  |                  IAirdrop, ReentrancyGuard                   |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                 authorizeWallet                  |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                  allowClaiming                   |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                   claimAirdrop                   |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                   isAuthorized                   |                          Public ❗️                          |                |             NO❗️             |
|             └              |                 numberAuthorized                 |                          Public ❗️                          |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|    **BootstrapBallot**     |                  Implementation                  |              IBootstrapBallot, ReentrancyGuard               |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                       vote                       |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                  finalizeBallot                  |                         External ❗️                         |       🛑       |         nonReentrant          |
|                            |                                                  |                                                              |                |                               |
|  **InitialDistribution**   |                  Implementation                  |                     IInitialDistribution                     |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |               distributionApproved               |                         External ❗️                         |       🛑       |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|       **PoolUtils**        |                     Library                      |                                                              |                |                               |
|             └              |                     \_poolID                     |                         Internal 🔒                          |                |                               |
|             └              |                \_poolIDAndFlipped                |                         Internal 🔒                          |                |                               |
|             └              |               \_placeInternalSwap                |                         Internal 🔒                          |       🛑       |                               |
|                            |                                                  |                                                              |                |                               |
|      **PoolsConfig**       |                  Implementation                  |                    IPoolsConfig, Ownable                     |                |                               |
|             └              |                  whitelistPool                   |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |                 unwhitelistPool                  |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |          changeMaximumWhitelistedPools           |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |    changeMaximumInternalSwapPercentTimes1000     |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |             numberOfWhitelistedPools             |                         External ❗️                         |                |             NO❗️             |
|             └              |                  isWhitelisted                   |                          Public ❗️                          |                |             NO❗️             |
|             └              |                 whitelistedPools                 |                         External ❗️                         |                |             NO❗️             |
|             └              |               underlyingTokenPair                |                         External ❗️                         |                |             NO❗️             |
|             └              |             tokenHasBeenWhitelisted              |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|       **PoolStats**        |                  Implementation                  |                          IPoolStats                          |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |           \_updateProfitsFromArbitrage           |                         Internal 🔒                          |       🛑       |                               |
|             └              |               clearProfitsForPools               |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                   \_poolIndex                    |                         Internal 🔒                          |                |                               |
|             └              |             updateArbitrageIndicies              |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |           \_calculateArbitrageProfits            |                         Internal 🔒                          |                |                               |
|             └              |            profitsForWhitelistedPools            |                         External ❗️                         |                |             NO❗️             |
|             └              |                arbitrageIndicies                 |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|         **Pools**          |                  Implementation                  | IPools, ReentrancyGuard, PoolStats, ArbitrageSearch, Ownable |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |   ArbitrageSearch PoolStats   |
|             └              |                   setContracts                   |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |              startExchangeApproved               |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                  \_addLiquidity                  |                         Internal 🔒                          |       🛑       |                               |
|             └              |                   addLiquidity                   |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                 removeLiquidity                  |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                     deposit                      |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                     withdraw                     |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |             \_adjustReservesForSwap              |                         Internal 🔒                          |       🛑       |                               |
|             └              |                   \_arbitrage                    |                         Internal 🔒                          |       🛑       |                               |
|             └              |        \_determineSwapAmountInValueInETH         |                         Internal 🔒                          |                |                               |
|             └              |                \_attemptArbitrage                |                         Internal 🔒                          |       🛑       |                               |
|             └              |    \_adjustReservesForSwapAndAttemptArbitrage    |                         Internal 🔒                          |       🛑       |                               |
|             └              |                       swap                       |                         External ❗️                         |       🛑       | nonReentrant ensureNotExpired |
|             └              |               depositSwapWithdraw                |                         External ❗️                         |       🛑       | nonReentrant ensureNotExpired |
|             └              |            depositDoubleSwapWithdraw             |                         External ❗️                         |       🛑       | nonReentrant ensureNotExpired |
|             └              |                 getPoolReserves                  |                          Public ❗️                          |                |             NO❗️             |
|             └              |               depositedUserBalance               |                          Public ❗️                          |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|        **PoolMath**        |                     Library                      |                                                              |                |                               |
|             └              |               \_mostSignificantBit               |                         Internal 🔒                          |                |                               |
|             └              |                   \_maximumMSB                   |                         Internal 🔒                          |                |                               |
|             └              |                 \_zapSwapAmount                  |                         Internal 🔒                          |                |                               |
|             └              |             \_determineZapSwapAmount             |                         Internal 🔒                          |                |                               |
|                            |                                                  |                                                              |                |                               |
|   **CoreChainlinkFeed**    |                  Implementation                  |                          IPriceFeed                          |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |               latestChainlinkPrice               |                          Public ❗️                          |                |             NO❗️             |
|             └              |                   getPriceBTC                    |                         External ❗️                         |                |             NO❗️             |
|             └              |                   getPriceETH                    |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|    **CoreUniswapFeed**     |                  Implementation                  |                          IPriceFeed                          |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |               \_getUniswapTwapWei                |                          Public ❗️                          |                |             NO❗️             |
|             └              |                getUniswapTwapWei                 |                          Public ❗️                          |                |             NO❗️             |
|             └              |                   getTwapWBTC                    |                          Public ❗️                          |                |             NO❗️             |
|             └              |                   getTwapWETH                    |                          Public ❗️                          |                |             NO❗️             |
|             └              |                   getPriceBTC                    |                         External ❗️                         |                |             NO❗️             |
|             └              |                   getPriceETH                    |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|    **PriceAggregator**     |                  Implementation                  |                  IPriceAggregator, Ownable                   |                |                               |
|             └              |                 setInitialFeeds                  |                          Public ❗️                          |       🛑       |           onlyOwner           |
|             └              |                   setPriceFeed                   |                          Public ❗️                          |       🛑       |           onlyOwner           |
|             └              | changeMaximumPriceFeedPercentDifferenceTimes1000 |                          Public ❗️                          |       🛑       |           onlyOwner           |
|             └              |       changePriceFeedModificationCooldown        |                          Public ❗️                          |       🛑       |           onlyOwner           |
|             └              |               \_absoluteDifference               |                         Internal 🔒                          |                |                               |
|             └              |                \_aggregatePrices                 |                         Internal 🔒                          |                |                               |
|             └              |                  \_getPriceBTC                   |                         Internal 🔒                          |                |                               |
|             └              |                  \_getPriceETH                   |                         Internal 🔒                          |                |                               |
|             └              |                   getPriceBTC                    |                         External ❗️                         |                |             NO❗️             |
|             └              |                   getPriceETH                    |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|     **CoreSaltyFeed**      |                  Implementation                  |                          IPriceFeed                          |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                   getPriceBTC                    |                         External ❗️                         |                |             NO❗️             |
|             └              |                   getPriceETH                    |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|     **RewardsConfig**      |                  Implementation                  |                   IRewardsConfig, Ownable                    |                |                               |
|             └              |         changeRewardsEmitterDailyPercent         |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |           changeEmissionsWeeklyPercent           |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |           changeStakingRewardsPercent            |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |           changePercentRewardsSaltUSDS           |                         External ❗️                         |       🛑       |           onlyOwner           |
|                            |                                                  |                                                              |                |                               |
|       **Emissions**        |                  Implementation                  |                          IEmissions                          |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                  performUpkeep                   |                         External ❗️                         |       🛑       |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|     **RewardsEmitter**     |                  Implementation                  |               IRewardsEmitter, ReentrancyGuard               |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                  addSALTRewards                  |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                  performUpkeep                   |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |              pendingRewardsForPools              |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|      **SaltRewards**       |                  Implementation                  |                         ISaltRewards                         |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |               \_sendStakingRewards               |                         Internal 🔒                          |       🛑       |                               |
|             └              |              \_sendLiquidityRewards              |                         Internal 🔒                          |       🛑       |                               |
|             └              |          \_sendInitialLiquidityRewards           |                         Internal 🔒                          |       🛑       |                               |
|             └              |           \_sendInitialStakingRewards            |                         Internal 🔒                          |       🛑       |                               |
|             └              |              sendInitialSaltRewards              |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                  performUpkeep                   |                         External ❗️                         |       🛑       |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|          **USDS**          |                  Implementation                  |                    ERC20, IUSDS, Ownable                     |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             ERC20             |
|             └              |            setCollateralAndLiquidity             |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |                      mintTo                      |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |               burnTokensInContract               |                         External ❗️                         |       🛑       |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|      **StableConfig**      |                  Implementation                  |                    IStableConfig, Ownable                    |                |                               |
|             └              |     changeRewardPercentForCallingLiquidation     |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |    changeMaxRewardValueForCallingLiquidation     |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |     changeMinimumCollateralValueForBorrowing     |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |       changeInitialCollateralRatioPercent        |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |       changeMinimumCollateralRatioPercent        |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |    changePercentArbitrageProfitsForStablePOL     |                         External ❗️                         |       🛑       |           onlyOwner           |
|                            |                                                  |                                                              |                |                               |
| **CollateralAndLiquidity** |                  Implementation                  |              Liquidity, ICollateralAndLiquidity              |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |           Liquidity           |
|             └              |        depositCollateralAndIncreaseShare         |                         External ❗️                         |       🛑       | nonReentrant ensureNotExpired |
|             └              |            withdrawCollateralAndClaim            |                         External ❗️                         |       🛑       | nonReentrant ensureNotExpired |
|             └              |                    borrowUSDS                    |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                    repayUSDS                     |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                  liquidateUser                   |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |            underlyingTokenValueInUSD             |                          Public ❗️                          |                |             NO❗️             |
|             └              |            totalCollateralValueInUSD             |                          Public ❗️                          |                |             NO❗️             |
|             └              |             userCollateralValueInUSD             |                          Public ❗️                          |                |             NO❗️             |
|             └              |            maxWithdrawableCollateral             |                          Public ❗️                          |                |             NO❗️             |
|             └              |                maxBorrowableUSDS                 |                          Public ❗️                          |                |             NO❗️             |
|             └              |          numberOfUsersWithBorrowedUSDS           |                          Public ❗️                          |                |             NO❗️             |
|             └              |               canUserBeLiquidated                |                          Public ❗️                          |                |             NO❗️             |
|             └              |              findLiquidatableUsers               |                          Public ❗️                          |                |             NO❗️             |
|             └              |              findLiquidatableUsers               |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|       **Liquidizer**       |                  Implementation                  |                     ILiquidizer, Ownable                     |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                   setContracts                   |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |              incrementBurnableUSDS               |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                    \_burnUSDS                    |                         Internal 🔒                          |       🛑       |                               |
|             └              |                \_possiblyBurnUSDS                |                         Internal 🔒                          |       🛑       |                               |
|             └              |                  performUpkeep                   |                         External ❗️                         |       🛑       |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|     **StakingConfig**      |                  Implementation                  |                   IStakingConfig, Ownable                    |                |                               |
|             └              |              changeMinUnstakeWeeks               |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |              changeMaxUnstakeWeeks               |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |             changeMinUnstakePercent              |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |            changeModificationCooldown            |                         External ❗️                         |       🛑       |           onlyOwner           |
|                            |                                                  |                                                              |                |                               |
|       **Liquidity**        |                  Implementation                  |                  ILiquidity, StakingRewards                  |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |        StakingRewards         |
|             └              |               \_dualZapInLiquidity               |                         Internal 🔒                          |       🛑       |                               |
|             └              |        \_depositLiquidityAndIncreaseShare        |                         Internal 🔒                          |       🛑       |                               |
|             └              |           \_withdrawLiquidityAndClaim            |                         Internal 🔒                          |       🛑       |                               |
|             └              |         depositLiquidityAndIncreaseShare         |                         External ❗️                         |       🛑       | nonReentrant ensureNotExpired |
|             └              |            withdrawLiquidityAndClaim             |                         External ❗️                         |       🛑       | nonReentrant ensureNotExpired |
|                            |                                                  |                                                              |                |                               |
|     **StakingRewards**     |                  Implementation                  |               IStakingRewards, ReentrancyGuard               |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |               \_increaseUserShare                |                         Internal 🔒                          |       🛑       |                               |
|             └              |               \_decreaseUserShare                |                         Internal 🔒                          |       🛑       |                               |
|             └              |                 claimAllRewards                  |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                  addSALTRewards                  |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |               totalSharesForPools                |                         External ❗️                         |                |             NO❗️             |
|             └              |               totalRewardsForPools               |                         External ❗️                         |                |             NO❗️             |
|             └              |                userRewardForPool                 |                          Public ❗️                          |                |             NO❗️             |
|             └              |               userRewardsForPools                |                         External ❗️                         |                |             NO❗️             |
|             └              |                 userShareForPool                 |                          Public ❗️                          |                |             NO❗️             |
|             └              |                userShareForPools                 |                         External ❗️                         |                |             NO❗️             |
|             └              |            userVirtualRewardsForPool             |                          Public ❗️                          |                |             NO❗️             |
|             └              |                  userCooldowns                   |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|        **Staking**         |                  Implementation                  |                   IStaking, StakingRewards                   |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |        StakingRewards         |
|             └              |                    stakeSALT                     |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                     unstake                      |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                  cancelUnstake                   |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |                   recoverSALT                    |                         External ❗️                         |       🛑       |         nonReentrant          |
|             └              |       transferStakedSaltFromAirdropToUser        |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                    userXSalt                     |                         External ❗️                         |                |             NO❗️             |
|             └              |                 unstakesForUser                  |                          Public ❗️                          |                |             NO❗️             |
|             └              |                 unstakesForUser                  |                         External ❗️                         |                |             NO❗️             |
|             └              |                  userUnstakeIDs                  |                         External ❗️                         |                |             NO❗️             |
|             └              |                   unstakeByID                    |                         External ❗️                         |                |             NO❗️             |
|             └              |                 calculateUnstake                 |                          Public ❗️                          |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|     **ManagedWallet**      |                  Implementation                  |                        IManagedWallet                        |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                  proposeWallets                  |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                 <Receive Ether>                  |                         External ❗️                         |       💵       |             NO❗️             |
|             └              |                  changeWallets                   |                         External ❗️                         |       🛑       |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|     **AccessManager**      |                  Implementation                  |                        IAccessManager                        |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |             excludedCountriesUpdated             |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                  \_verifyAccess                  |                         Internal 🔒                          |                |                               |
|             └              |                   grantAccess                    |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                 walletHasAccess                  |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|          **Salt**          |                  Implementation                  |                         ISalt, ERC20                         |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             ERC20             |
|             └              |               burnTokensInContract               |                         External ❗️                         |       🛑       |             NO❗️             |
|             └              |                   totalBurned                    |                         External ❗️                         |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|      **SigningTools**      |                     Library                      |                                                              |                |                               |
|             └              |                \_verifySignature                 |                         Internal 🔒                          |                |                               |
|                            |                                                  |                                                              |                |                               |
|         **Upkeep**         |                  Implementation                  |                   IUpkeep, ReentrancyGuard                   |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                      step1                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step2                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                    \_formPOL                     |                         Internal 🔒                          |       🛑       |                               |
|             └              |                      step3                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step4                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step5                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step6                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step7                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step8                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step9                       |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step10                      |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                      step11                      |                          Public ❗️                          |       🛑       |       onlySameContract        |
|             └              |                  performUpkeep                   |                          Public ❗️                          |       🛑       |         nonReentrant          |
|             └              |      currentRewardsForCallingPerformUpkeep       |                          Public ❗️                          |                |             NO❗️             |
|                            |                                                  |                                                              |                |                               |
|     **ExchangeConfig**     |                  Implementation                  |                   IExchangeConfig, Ownable                   |                |                               |
|             └              |                  <Constructor>                   |                          Public ❗️                          |       🛑       |             NO❗️             |
|             └              |                   setContracts                   |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |                 setAccessManager                 |                         External ❗️                         |       🛑       |           onlyOwner           |
|             └              |                 walletHasAccess                  |                         External ❗️                         |                |             NO❗️             |

Legend

| Symbol | Meaning                   |
| :----: | ------------------------- |
|   🛑   | Function can modify state |
|   💵   | Function is payable       |

</div>
____
<sub>
Thinking about smart contract security? We can provide training, ongoing advice, and smart contract auditing. [Contact us](https://diligence.consensys.net/contact/).
</sub>
