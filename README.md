#
# **CHAINLINK SPRING 2022 HACKATHON: INVENIAM CHALLENGES INSTRUCTIONS**

Welcome to Inveniam&#39;s Hackathon Challenges for Chainlink Spring 2022 Hackathon! The challenges presented below involve creating novel solutions for the emerging decentralized finance space. If you choose to take on these challenges, you will be working between the platforms of multiple companies spearheading the global trading of tokenized assets! These companies include Inveniam, Tokeny, Blockportal, Accumulate, and Chainlink.


## **Things To Note**

1. These hackathon challenges are available on the **Polygon Testnet (Mumbai)**.
2. You may participate in one or both challenges.
3. To register with Inveniam for these challenges please join the **BlockPortal Discord Server** where there are channels for the Chainlink Hackathon.
  1. Discord Invite: [https://discord.gg/swZw7fbax4](https://discord.gg/swZw7fbax4)
4. Please direct any questions or comments regarding the hackathon challenges to the BlockPortal Discord channels where team members will be available to assist you.
5. To gain access to the credentials used for these Hackathon challenges, you must join the BlockPortal Discord Server and be assigned the role of &quot;hacker&quot; by a team member.


## **Setting the Stage**

- **Property XYZ** is a multifamily apartment complex
- The owner of Property XYZ wanted to increase the **liquidity** of their real estate asset, so they decided to **tokenize** the equity relating to the asset
- The owner utilized **Inveniam** to credential the documents relating to Property XYZ and began conducting quarterly appraisals
- Cryptographic proofs of the documents (JSONs) related to the property were hashed onto the **Accumulate** blockchain, with anchors written to **Polygon**
- Shares representing the equity of Property XYZ were tokenized into **1000 security tokens** using **Tokeny**
- **52 accredited investors** with **ONCHAINID&#39;s** purchased varying amounts of the security token, entitling them to a portion of Property XYZ&#39;s equity
- After one quarter had passed, the valuation of Property XYZ had increased so the owner is required to pay out a **distribution totaling 46,261.65 USDX** to all shareholders

![Inveniam Hackathon Tokenization](https://uploads-ssl.webflow.com/61e1c00981eb8551acfd7317/626c1c03c09fb291930dc9f3_Inveniam%20Hackathon%20Tokenization.png)


## **The Challenges**

### **Challenge 1: Use a Smart Contract to send a message to holders of a security token.**

Just like shareholders in public companies, holders of Security Tokens want to receive periodic messages, notices, and reports from &quot;management.&quot; In this challenge, you will use a smart contract, connected via Chainlink, to manage a &quot;notice of distribution&quot; (dividend) sent by the management of a Tokeny Security token.

The message will be personalized based on the tokenholders&#39; share, dividing the total value of the distribution based on that share. Either of two messaging methods can be used: Alternative (a) Send messages via Tokeny&#39;s secure messaging system; Alternative (b) Retrieve a list of email addresses from Tokeny and send each a personalized notice via email.

The winning entry will be a dApp/smart contract that uses Chainlink&#39;s oracle and smart contract functions to integrate the function of: a JSON Transaction file, Tokeny (OnChainID for investors), and uses the single-source Chainlink node managed by BlockPortal.

### **Challenge 2: Use a Smart Contract to Pay a dividend via stablecoin to holders of a security token.**

Just like shareholders in public companies, holders of Security Tokens want to receive periodic income from their investments. In this challenge, you will use a smart contract, connected via Chainlink, to manage the simple computation and on-chain payment of a dividend sent by the management of a Tokeny Security token.

The Token&#39;s total dividend payment of $46,261.65 will be divided between token holders according to the share they own. The payment will be delivered via a stablecoin (USDX) into a separate investor wallet, similar to how shareholders of a stock are paid into a separate cash account.

The winning entry will be a dApp/smart contract that uses Chainlink&#39;s oracle and smart contract functions to integrate the function of: a JSON Transaction file, Tokeny (OnChainID for investors), and uses the single-source Chainlink node managed by BlockPortal.


## **Sample High-Level Workflow**

![Inveniam Hackathon High-Level Workflow](https://uploads-ssl.webflow.com/61e1c00981eb8551acfd7317/626c1c0345c0fe8ab97aaea1_Inveniam%20Hackathon%20Workflow.png)


## **Assets and Links**

### **Accumulate Protocol (ACME)** **(**[**https://accumulatenetwork.io/**](https://accumulatenetwork.io/)**)**

A low cost, high volume storage of event logs (currently operating as the Factom chain) used internally by Inveniam to record asset performance.

- **Identity Proof JSON**
  - [https://gitlab.com/accumulatenetwork/sdk/anchor-solidity/-/blob/main/identity\_proof\_compact.json](https://gitlab.com/accumulatenetwork/sdk/anchor-solidity/-/blob/main/identity_proof_compact.json)
- **Proving the Proof**
  - Guide: [https://gitlab.com/accumulatenetwork/sdk/anchor-solidity](https://gitlab.com/accumulatenetwork/sdk/anchor-solidity)

### **Inveniam (**[**https://inveniam.io/**](https://inveniam.io/)**)**

The Inveniam.io system is where the message to investors will be generated and approved by Management of the investment. Inveniam.io provides Asset management, Workflow, and DLT proof of: documents, values, and transactions.

- **Property Owner/Manager**
  - Issuer/Event Wallet for distribution payment
    - Polygon (Mumbai)
      - Address: [0x78d7164e7c38d2bd577746b7ad14cd682a26539c](https://urldefense.proofpoint.com/v2/url?u=https-3A__blockscan.com_address_0x78d7164e7c38d2bd577746b7ad14cd682a26539c&amp;d=DwMFaQ&amp;c=euGZstcaTDllvimEN8b7jXrwqOf-v5A_CdpgnVfiiMM&amp;r=wwMDO-PpcsKYfuukO0-WtcUCFTergulK4hjUC-ONpkg&amp;m=bQN8M5I6d6ZhJ9VDjJox5i9KIGt4e8GhsuPfH5KNSJw&amp;s=GsXYBbcNDYtarg4x-HLCQO6eCubyrcCDBuGj03AtBxM&amp;e=)
- **Investors**
  - Email inbox (for QA purposes only)
    - [https://www.google.com/gmail/](https://www.google.com/gmail/)
    - Credentials: [https://discord.gg/swZw7fbax4](https://discord.gg/swZw7fbax4)
- **Notification and Distribution Data**
  - Notification JSON
    - Polygon (Mumbai)
      - Checksum: df40050ead01fcb1fb1a46372200d6df76526d1aa815d560d10baf01009a0766
      - Contract: [0x0b297f5896ba9d4c13ab84ebccf501fed229ac594c1c4387e9058a2e7adabe3a](https://mumbai.polygonscan.com/tx/0x0b297f5896ba9d4c13ab84ebccf501fed229ac594c1c4387e9058a2e7adabe3a)
  - **Distribution JSON**
    - Polygon (Mumbai)
      - Checksum:
      - Contract: [0x9856e4115bfd48a32ffd551b2473ee56f5f16bd92cd234a13c7e5d155057a363](https://mumbai.polygonscan.com/tx/0x9856e4115bfd48a32ffd551b2473ee56f5f16bd92cd234a13c7e5d155057a363)

### **Tokeny (**[**https://tokeny.com/**](https://tokeny.com/)**)**

A Tokeny security token records the identities and secure addresses of token holders, thereby creating security tokens that are compliant with local securities laws. Tokeny provides most &quot;Investor relations&quot; functions that are traditional in public companies but are unusual for digital assets. Specifically, Tokeny provides Management of the &quot;Cap Table&quot; showing which investors own how much of the company at any given time. The Cap Table allows for dividing ownership and dividends between investors. Tokeny also supplies Anti-Money Laundering (AML) and Know Your Customer (KYC) checks on investment holders to ensure that they came by their money legally, and are using it for legal functions.

- **Equity Tokens**
  - Polygon (Mumbai)
    - Name: CLink0422 POLYGON
    - Symbol: CLPOLY
    - Circulating supply: 1000
    - Smart contract: [0x70f9c5b6a4cb603723fd30526a5b8f446079a690](https://mumbai.polygonscan.com/token/0x70f9c5b6a4cb603723fd30526a5b8f446079a690)
- **Tokeny Servicing API**
  - Polygon (Mumbai)
    - API endpoints will need to point to **servicing-api-testing**
    - Credentials: [https://discord.gg/swZw7fbax4](https://discord.gg/swZw7fbax4)
  - API Documentation: https://tokeny-solutions.readme.io/reference
- **ONCHAINID**
  - Smart Contract Documentation: [https://github.com/onchain-id/solidity](https://github.com/onchain-id/solidity)

### **Chainlink (**[**https://chain.link/**](https://chain.link/)**)**

- **Chainlink Node**
  
  Reference documentation for Chainlink large bytes request/response: <https://ijonas.com/fetching-large-responses-with-chainlink-anyapi>

  - Polygon (Mumbai)
    - Node account address: `0x6C65C2586b52172fa71034c4002c2BFbE7C9e8F6`
    - Operator contract: `0xa16DA7EF5DC9F124a030c473c457d41e287CBBb4`
    - External Job Id (Spec Id): `2c23d622-68f3-4603-b4d6-1afcd16feddc` (Use without dashes: `2c23d62268f34603b4d61afcd16feddc`)
