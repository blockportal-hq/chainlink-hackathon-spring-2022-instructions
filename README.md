# chainlink-hackathon-spring-2022-instructions


CHALLENGES 

Challenge 1:  
Use a Smart Contract to send a message to a holders of a security token. 

Just like shareholders in public companies, holders of Security Tokens want to receive periodic messages, notices, and reports from "management."  In this challenge, you will use a smart contract, connected via Chainlink, to manage a "notice of distribution" (dividend) sent by the management of a Tokeny Security token.   

The message will be personalized based on the tokenholders' share, dividing the total value of the distribution based on that share. Either of two messaging methods can be used: Alternative (a) Send messages via Tokeny's secure messaging system; Alternative (b) Retrieve a list of email addresses from Tokeny and send each a personalized notice via email. 

The winning entry will be a smart contract that uses Chainlink's oracle and smart contract functions to integrate the function of: Inveniam.io (DLT-validated Investment management), Tokeny.com (OnChainID for investors), and Chainlink and use the functions of blockportal.com. 

 

In the challenge example. a group of apartments has been tokenized and fractionalized and would like to send a notice to its token holders that they will soon receive their fair share of a dividend payment. 

Challenge 2: 
Use a Smart Contract to Pay a dividend via stablecoin to holders of a security token. 

Just like shareholders in public companies, holders of Security Tokens want to receive periodic income from their investments.  In this challenge, you will use a smart contract, connected via Chainlink, to manage the simple computation and on-chain payment of a dividend sent by the management of a Tokeny Security token.   

The Token's total dividend payment will be divided between token holders according to the share they own.  The payment will be delivered via a stablecoin (simulated for this challenge) into a separate investor wallet, similar to how shareholders of a stock are paid into a separate cash account. 

The winning entry will be a smart contract that uses chain.link's oracle and smart contract functions to integrate the function of: Inveniam.io (DLT-validated Investment management), Tokeny.com (OnChainID for investors), and Chain.Link and use the functions of blockportal.com. 

 

In the challenge example. a group of apartments has been tokenized and fractionalized and would like to declare a dividend worth about USD 11,000 in total and divide it among its tokenholders (of a Tokeny security token) 

 

Page Break
 

TECHNOLOGY PARTNERS 

Accumulate Protocol (ACME) (https://accumulatenetwork.io/) 

A Low cost, high volume storage of event logs (currently operating as the Factom chain) used internally by Inveniam to record asset performance 

Inveniam.io (inveniam.io) 

The Inveniam.io system is where the message to investors will be generated and approved by Management of the investment. Inveniam.io provides Asset management, Workflow, and DLT proof of: documents, values, and transactions. 

Tokeny (tokeny.com) 

A Tokeny security token records the identities and secure addresses of tokenholders, thereby creating security tokens  that are compliant with local securities laws.  Tokeny provides most "Investor relations" functions that are traditional in public companies but are unusual for digital assets.  Specifically, Tokeny provides Management of the "Cap Table" showing which investors own how much of the company at any given time.  The Cap Table allows for  dividing ownership and dividends between investors.  Tokeny also supplies Anti-Money Laundering (AML) and Know Your Customer (KYC) checks on investment holders to ensure that they came by their money legally, and are using it for legal functions.   

Token Exchange (Alternative Trading Systems) 

Alternative Trading Systems allow a token to be bought/sold in a marketplace after issuance.  In our example, it may be that a token has changed owners since it was issued, and that this information will have been given to Tokeny to update the "cap table" (a company's listing of its shareholders). Examples include: 

Oasis Pro Markets (oasispromarkets.com) 

MakerDAO (makerdao.com) 

Rialto (rialtomarkets.com) 

Page Break
 

FLOWCHART & DESCRIPTION (see lucidchart ) 

Inveniam Asset Management 

Inveniam provides a platform for creating a verified record of an asset's existence off-chain the legal, financial, or physical world.  Assets like companies or real estate are known via their legal documents, operational data (including IoT/sensors where available), and their financial data (as provided by Management) 

Asset onboarded 

Onboarding an asset involves identifying an asset by its name, its type, its corporate form, its management team, and the workflows required to keep its data current and accurate.  A page is created for each asset, along with related pages for managing the asset. 

Creation of a Federated Data Room (a deal room owned by the asset) 

While not directly part of the challenge, there is a data room, owned by the Token’s Management that stores documents and data associated with the performance of the underlying asset (such as that it has excess cash that can be paid out) and recording management’s decisions (such as that a dividend will be paid in a certain amount on a certain date). 

Identification of a team that manages the tokenized asset 

The team that manages an asset includes roles that are authorized to report and approve financial performance and to approve and pay dividends.   

Identification of the data required to ascertain the asset's value and financial performance 

In order to pay a dividend, an asset should have a valuation (to determine its value) and records of financial performance to determine the amount of available funds for paying a cash dividend. 

Definition of the ongoing processes needed to maintain the asset 

Assets may differ on the kinds of information needed to support a valuation and report performance, but whatever these are, the Inveniam.io system defines a workflow that supports the updating, review and valuation of an asset. 

Documents uploaded and anchored to blockchain 

Documents typically include legal and contractual PDFs and spreadsheets or reports of financial performance.   

For real estate documents can also include leases, tax information, surveys, flood maps, site photos, and market comparable data. 

Real estate investments may also be structured as limited partnerships holding equity or debt associated with the underlying real estate. 

Data artifacts created 

A Data Artifact is a data structure containing the normalized data associated. These data artifacts are reviewed, onboarded to Inveniam.io and Asset value/mark is set according to details provided in valuation report (1.4). The asset's value is stored and a supporting hash is written to the appropriate blockchain/DLT. 

Valuation report created by valuation agent 

For Real Estate assets, the valuation is an appraisal performed by a licensed appraiser.  The appraisal report is received by Inveniam, extracted, and both the document and its data artifact are hashed and the hash is written to the appropriate blockchain/DLT. 

Asset value/mark set 

Asset value/mark is set according to details provided in valuation report (1.4). The asset's value is stored and a supporting hash is written to the appropriate blockchain/DLT. 

Tokenization requirements set 

 

Number of shares authorized and issued 

Classes of share ownership (preferred, common, limited partners) 

List of shareholders and position classes and sizes 

Tokeny Investor Management 

Tokeny is a platform for issuing tokens that conform to and comply with national laws and regulations around the issuance and marketing of securities. 

 

Asset tokenized based on requirements (Tokeny security token / smart contract) 

A Tokeny Security Token is designed to both reflect the security (financial contract) and the underlying asset (such as income-producing real estate) and for its legal provisions to meet local securities law. (Investopedia: What are Investment Securities?) 

Tokeny investor and distribution functions 

Initial investors onboarded to Tokeny, assigned OnChainID 

Tokeny.com has a unique solution--the OnChainID--that bridges the gap between crypto-anonymity and the need for a verified personal identity.   

OnChainIDs are stored on the public Ethereum BlockChain, in a decentralized way. They can't be hidden nor deleted. No service or organization can remove an identity owner's access rights to it. 

Identities are smart contracts, deployed on the Polygon Network (https://polygon.technology/). Any implementation standard to the ERC734 and ERC735 proposals are supported by the ONCHAINID standard, and thus with any service that supports the ONCHAINID standard too.' 

The OnChainID allows compliance with all applicable securities regulations. Regulated exchanges require market participants to have an ID, linked to an existing person or organization. Proof of this information is called a Claim. 

Claims are issued by any Claim Issuer that is allowed by the Identity Owner to publish claims about the Identity. For example, a Claim Issuer could emit a claim saying that a given Identity has passed an Identity Check with an ID card and a selfie. 

Senstive information such as government-issued ID card number or the picture itself is not stored on the blockchain publicly. The Claim Issuer will store the claim Private Data on its off-chain servers and will publish a signature publicly onchain. Therefore, anyone knows that a trusted third party has successfully checked the identity. But to access the data, one would need the explicit consent of the Identity Owner. 

Learn more: https://docs.tokeny.com/docs/onchain-identities 

Anti-money-laundering (AML) & Know Your Customer (KYC) 

AML - refers to the activities performed to achieve compliance with legal requirements to actively monitor for and report suspicious activities. 

KYC – set of standards that ensures detailed information about clients' risk tolerance, investment knowledge, and financial position is known. 

Identities stored near-chain  (how Tokeny handles Personally Identifiable Information (PII)) 

OnChainID created 

Tokeny OnChainID description (https://docs.tokeny.com/docs/onchain-identities) 

 

Initial Security Tokens distributed to existing shareholders 

Distribution of security token to Exchanges (Alternative Trading Systems) 

Ongoing trading between investors after initial offering 

New investors (potential buyers) onboarded to Tokeny 

 

Trading of token on exchanges 

 

An existing investor offers fractional token for sale 

A Tokeny-validated investor buys the token fractions 

T-REX Tokeny transfers ownership between OnchainIDs 

https://docs.tokeny.com/docs/smart-contractsA 

Inveniam Valuation as a Service (Ongoing, Periodic) 

Inveniam's Valuation as a Service requires the periodic updating of the documents and financial reports to inform the periodic re-valuation of an asset.  As part of this process, asset-owners can also document excess earnings that they wish to return to investors.  Different capital structures require different methods to distribute excess earnings, but all are basically like the process by which a corporation declares a dividend. 

As a Proof of Process, the Inveniam Valuation as a Service steps includes an ongoing storage of the sequence of events onto the Accumulate blockchain. 

New asset documents uploaded (as an ongoing, periodic process) 

 

New data artifacts created (repeats step 1.3) 

The Data Artifacts are data structures containing the normalized data associated. These data artifacts are reviewed, onboarded to Inveniam.io and Asset value/mark is set according to details provided in valuation report (1.4). The asset's value is stored and a supporting hash is written to the appropriate blockchain/DLT. 

New Valuation report created (repeats step 1.4) 

For Real Estate assets, the valuation is an appraisal performed by a licensed appraiser.  The appraisal report is received by Inveniam, extracted, and both the document and its data artifact are hashed and the hash is written to the appropriate blockchain/DLT. 

New asset value/mark set (repeats step 1.5) 

Asset value/mark is set according to details provided in valuation report (1.4). The asset's value is stored and a supporting hash is written to the appropriate blockchain/DLT. 

Inveniam Investor Calculations (Waterfall as a Service) 

What is a Waterfall?  Why is it  a key process relating an investment, the investment's manager, and the many investors? 

If the same asset has issued multiple securities (debt vs equity, preferred vs common shares, classes within types) then a calculation has to be run to determine how they will divide the securities' income between them.  This is the Waterfall calculation (Investopedia: What is a Waterfall) 

Manager determines there will be a distribution 

A manager reviews recent financial performance and decides that there is enough excess income that some of it can be distributed to investors.  The manager makes an Investment-level notice to declare that a lump sum will be distributed to investors and divided between them according to shares.  

Allocations to share class are determined 

( 

WaaS distribution output per share class 

A successful waterfall will produce… 

Board approves distribution 

The distribution/payout/dividend needs to be approved again once it has been calculated at the investor level 

Distribution notice created for a share class 

 Form letter and data table 

Data anchored (Trigger) 

 Notice to smart contract 

Distribution event triggered 

(Marin & Kevin & Jeff) 

Distribution event received 

  

Distribution smart contracts initiated by the HUB 

 

Distribution event received and data received 

Potential optimization for BlockPortal to fetch data on event  

Smart Contract Initiation and Data Retrieval 

 

Smart contract initiation 

 

By the HUB 

 Future 

By Hackathon 

 Hackathon – self initiate 

Smart contract requests Inveniam data from oracle 

 

Requests Inveniam data (json) from Chainlink Node 

It is important that the json be passed literally intact (exactly the same bits that were hashed) 

BlockPortal gets deal distribution information from Inveniam API (future state) 

Current state: BlockPortal has two JSON object in S3. Distribution notice JSON; Distribution details JSON (again, Json cannot be changed or reformatted in order to make sure hashes match) 

Data retrieved from BlockPortal and available for oracle/smart contract 

 

Verify the identity and data using anchor hashes on ETH/MATIC 

 

Retrieve investor wallets 

 

Using Blockchain ledger 

 

Using Tokeny smart contract 

 

Investor Dividend Amounts and Notices 

 

Calculate distribution amounts per investor 

 

Challenge 1 – Tokeny Message 

 

Compose distribution notice for each investor individually 

 

Send distribution notice to each investor using oracle and Tokeny API 

 

Post message(s) to Tokeny API using Chainlink/BlockPortal node 

 

Challenge 1 – Email 

 

Use the Tokeny API to GET contact information (email) for each investor 

 

Compose distribution notice for each investor individually 

 

Use an email client to send Distribution Notification to each investor 

 

Challenge 2 - Distribution of Stablecoins to Investors 

Investors own a Security Token, but expect their dividend in either fiat currency (Fiat) or cryptocurrency (Crypto) 

Verify funds in distribution event wallet 

 

Execute distribution from event wallet to each investor individually 

 

Other Functions 

 

Chainlink node physical creation (Dynamic Mining) 

 

Chainlink node begins operating 

 
