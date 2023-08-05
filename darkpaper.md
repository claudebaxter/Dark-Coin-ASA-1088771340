# Introduction

Dark Coin is an experimental grassroots community project focused on expanding the Algorand DeFi ecosystem. Managed by a decentralized autonomous organization (DAO), Dark Coin's users collectively own and manage the project based on blockchain-enforced rules and smart contracts. The primary objective of the Dark Coin DAO is to develop privacy solutions for the Algorand Network.

# Disclaimer

Investing in Dark Coin or any cryptocurrency involves risks. The project's creators and developers do not guarantee profits or specific price outcomes for the Dark Coin token. It's essential to conduct thorough research and consider seeking guidance from a financial advisor before investing. Never invest funds you cannot afford to lose.

# Dark Coin product description and proposed use cases

Dark Coin is developing a browser-based DApp accessible at https://dark-coin.com, enabling users to send and receive private transactions on the Algorand network. The public beta was launched on May 10, 2022. Through the governance protocol, users can influence the project's direction using NFT-based voting tokens. Watch the voting DApp demonstration video at https://vimeo.com/759600718/7a65b8b2a6.

# Dark Coin Transaction Mixer

As of October 10, 2022, the Dark Coin Transaction Mixer public beta has been released. Users are able to send transactions between wallets using the mixer to add a layer of privacy by obfuscating the connection between the sending and receiving wallets.

The mixer has been added to the Dark Coin app, which can be located at https://dark-coin.com and the repository for our app can be found at https://github.com/ToysToTinkerWith/DarkCoin. An instructional demonstration video can be found here: https://vimeo.com/763136434/83b69d100a and you can view the application on Algoexplorer here: https://algoexplorer.io/application/885581567. 

After connecting and opting in, our users can send 5 different pre-set amounts of Algos ranging from 5A to 500A (5A, 20A, 50A, 100A, and 500A). The user can select the amount they wish to send, and enter the recipients address and submit the transaction. Once the transaction is signed, the Algos will be sent to the mixer wallet address (43EVULWFT4RU2H7EZH377SAVQJSJO5NZP37N3Y5DZ7PGUXOETKW7VWDIOA). Once four transactions have been queued in the mixer for the same amount, the outgoing transactions are shuffled out to the receiving wallets. The amount of pending transactions in each option is displayed on dark-coin.com as well as the in the global state on the application (885581567).

To use the mixer, users have the option to pay the fees in Algorand at the rate of 2% of the total transaction, or can pay the fees using Dark Coin at the rate of 1%.

This process adds a layer of privacy to transactions. If you view these transactions on a platform like Algoexplorer, you can see transactions going into and out of the mixer, but would not be able to directly connect a specific sender wallet to a specific receiving wallet.

A technical summary/outline of the process looks like this:

   1. Once connected/opted in, the user selects the amount of Algos they wish to send, and chooses to pay 2% fees with Algos, or 1% fees with Dark Coin.
   2. The user enters the receiving wallet address with the GUI.
   3. When ready, the user must tap/click the "mix" button and sign the transaction.
   4. The receiving wallet is temporarily logged in an off-chain database and funds are sent to the mixer.*
   5. The confirmation round from the initial signed transaction is written into the database entry and paired to the receiving wallet.
   6. When enough transactions are queued, the receiving wallets are written in to the outgoing transactions in random order using a smart contract.
   7. Before the funds are shuffled out, the confirmation round records are verified to confirm the receiver wallet has not been altered in the database.
   8. If this verification check does not pass, the funds will be returned to the sending wallets.

*Please be aware that we are using a centralized database solution to store the recipient addresses to keep them "off chain" until the shuffle, to avoid the sender address from being linked directly to the recipient address. This is not a trustless/decentralized solution in the current form. The final version of this application will be, but we have not reached that stage of development yet. It is important to us for transparency that our users understand the inherent risks associated with a centralized solution. Our team does not want to mislead any of our users and wanted to be clear on these details.

*It is also important to note that once a "mix" has been shuffled out of the mixer, that the old database entries will be overwritten by the next batch of queued transactions sent into the mixer. The maximum number of transactions the mixer will accept in the queue is 16, so theoretically, the maximum number of records stored in the database will not exceed this number. 

Steps 7-8 are currently performed manually by Claude. If the verification check passes, the creator wallet signs off on the mix. We are working to automate this process, and potentially use the multi-sig feature as part of this process to increase security.

Mixer Disclaimer: Our transaction mixer does not provide 100% anonymity and we do not support the use of this application for any sort of criminal activity. This application only exists to add a reasonable degree of privacy to users who wish to send or receive Algos without the sender / receiver being directly linked. Imagine your regular bank account records--the general public cannot openly view your account history at any time, but the records are not 100% anonymous. Just like any monetary transaction, users of our app must ensure they are following the law at all times, and must keep their own records necessary to prove this to any governing entity. The developer team reserves the right to suspend/restrict the use of this application to any user/wallet at any time.

Support: For technical inquiries, please email the developer team at team@dark-coin.io. You can also message the subreddit moderator team at r/DarkCoinASA, or can join the Discord server here: https://discord.gg/xdZ6V5ybmq.

# Dark Coin AI Arena

Step into the innovative Dark Coin AI Arena, where creativity meets competition. Create unique character art NFTs using DALL·E AI, minted directly in your wallet. Craft character descriptions and define powerful attacks for your creations. Engage in thrilling battles against other users, wagering Dark Coin for a chance at victory. The AI generates captivating battle stories and selects a winner, who claims the wagered Dark Coin. Immerse yourself in a world of imagination and strategy, where your creations come to life and compete for glory and rewards.

# Dark Coin tokenomics

The Dark Coin V2 token was minted on April 20th, 2023, with a total supply of 500,000,000 tokens, up to 6 decimals. The asset number is 1088771340. The Dark Coin DAO approved a reimbursement action plan for users affected by the MyAlgo hack, utilizing V2 Dark Coin for reimbursement after the V2 liquidity pool was established. The Dark Coin V1 token was minted on the Algorand blockchain Saturday, February 12, 2022, with a total supply of 500,000,000 tokens.

With the original minting, 400,000,000 Dark Coin were transferred from the creator wallet to create the V1 liquidity pool on Tinyman so that users can exchange the asset, and can contribute additional liquidity to the pool to support the project. 

The remaining 100,000,000 tokens in the creator / developer wallets are used to disburse the early backer air drop, as well as future air drops & contest rewards the community decides to distribute (e.g., rewards to users for our logo contest). This will also be used to partner with other developers to help fund the development costs.

Profits earned from project NFT Sales will be split evenly between providing liquidity and the Marketing & Development wallet.

# Dark Coin developer wallet information

Asset Information on AlgoExplorer: https://algoexplorer.io/asset/601894079

Creator / Developer Wallet: AL6F3TFPSZPF3BSVUFDNOLMEKUCJJAA7GZ5GF3DN3Q4IVJVNUFK76PQFNE (darkcoin.algo)

Marketing & Development Wallet: 5QWEL3YRI4QA55BVTJYX6SACBULJPDI75SIG2YLC2T5LDOC3M7U5K3DTDQ

Liquidity Pool Wallet (Tinyman): 56XJVRGFUY5LJMUTRK4EOWOOPMW6HJI73XJVRAIFQZG5774ILJRLSOXKFM

# Dark Coin team

Anders Bergquist: Lead Blockchain Developer (Full-Stack)

Non-ExistentDomain: Systems Administrator

Ragingdragon: Community Manager

Claude Baxter: Front End Developer & ASA Creator
ASA Creator Linkedin: https://www.linkedin.com/in/claude-baxter-787229114
