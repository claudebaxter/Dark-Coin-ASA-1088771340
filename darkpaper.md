# Introduction

Dark Coin is an experimental grassroots community project to develop and expand the Algorand DEFI ecosystem. Dark Coin is managed by a decentralized autonomous organization (DAO), meaning that the project is collectively owned / managed by its users based on specific rules enforced by the blockchain and smart contracts. The Dark Coin DAOs main focus is developing privacy solutions for the Algorand Network.


# Disclaimer

There is no guarantee or promise made from the creator / developers that this project will make investors money. There is no guarantee or promise regarding the direction of the price action of the Dark Coin token.

Investing is always a risk. Anyone considering investing in this project, or crypto in general, should conduct thorough research and consider seeking guidance from a financial advisor. Never invest money that you cannot afford to lose.

# Dark Coin product description and proposed use cases

The Dark Coin team is developing a browser based DAPP located at https://dark-coin.com. Our users are able to send and receive private transactions on the Algorand network. The public beta has been released as of May 10, 2022. 

Being a DAO, the users of our dapp will also be able to use a governance protocol to make decisions on the projects direction/future. Our governance dApp will allow users to cast votes and submit proposals using NFT voting tokens. Here is a link to a demonstration video for the voting DAPP: https://vimeo.com/759600718/7a65b8b2a6.

# Dark Coin Transaction Mixer

As of October 10, 2022, the Dark Coin Transaction Mixer public beta has been released. Users are able to send transactions between wallets using the mixer to add a layer of privacy by obfuscating the connection between the sending and receiving wallets.

The mixer has been added to the Dark Coin app, which can be located at https://dark-coin.com and the repository for our app can be found at https://github.com/ToysToTinkerWith/DarkCoin. An instructional demonstration video can be found here: https://vimeo.com/763136434/83b69d100a and you can view the application on Algoexplorer here: https://algoexplorer.io/application/885581567. 

After connecting and opting in, our users can send 5 different pre-set amounts of Algos ranging from 5A to 500A (5A, 20A, 50A, 100A, and 500A). The user can select the amount they wish to send, and enter the recipients address and submit the transaction. Once the transaction is signed, the Algos will be sent to the mixer wallet address (43EVULWFT4RU2H7EZH377SAVQJSJO5NZP37N3Y5DZ7PGUXOETKW7VWDIOA). Once four transactions have been queued in the mixer for the same amount, the outgoing transactions are shuffled out to the receiving wallets. The amount of pending transactions in each option is displayed on dark-coin.com as well as the in the global state on the application (885581567).

To use the mixer, users have the option to pay the fees in Algorand at the rate of 2% of the total transaction, or can pay the fees using Dark Coin at the rate of 1%.

This process adds a layer of privacy to transactions. If you view these transactions on a platform like Algoexplorer, you can see transactions going into and out of the mixer, but would not be able to directly connect a specific sender wallet to a specific receiving wallet.

A technical summary/outline of the process looks like this:

   1. Once connected/opted in, the user selects the amount of Algos they wish to send, and enters the receiving wallet address with the GUI.
   2. The user chooses to pay 2% fees with Algos, or 1% fees with Dark Coin.
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

# Dark Coin tokenomics

Dark Coin was minted on the Algorand blockchain Saturday, February 12, 2022, with a total supply of 500,000,000 tokens.

400,000,000 Dark Coin was transferred from the creator wallet to create the liquidity pool on Tinyman so that users can exchange the asset, and can contribute additional liquidity to the pool to support the project. The LP tokens received for this have been locked through May 31, 2022, on Tinylock. Because we intend to keep this liquidity locked permanently, a new vote will be held before the end of May 2023 for the community to decide if we should continue to stay locked with Tinylock, or use another service, and for how long. This is simply to ensure that we are locking the liquidity in a way that is secure and responsible.

Users who locked in 5,000,000 Dark Coin by February 19, 2022 are provided with an initial early backer reward of 1,000,000 Dark Coin. The early backer program has concluded, and we are keeping this information in the darkpaper for transparency.

The remaining 100,000,000 tokens in the creator / developer wallets are used to disburse the early backer air drop, as well as future air drops & contest rewards the community decides to distribute (e.g., rewards to users for our logo contest). This will also be used to partner with other developers to help fund the development costs.

Profits earned from NFT Sales from the creator wallet will be split between providing liquidity and the Marketing & Development wallet.

Both the Creator and Developer Wallet 2 will not sell or transfer any of the initial 100,000,000 Dark Coin without disclosing details to the community for approval, as these funds are to be used to provide additional liquidity, as well as fund and promote the project as it expands.


# Dark Coin developer wallet information

Asset Information on AlgoExplorer: https://algoexplorer.io/asset/601894079

Creator / Developer Wallet: AL6F3TFPSZPF3BSVUFDNOLMEKUCJJAA7GZ5GF3DN3Q4IVJVNUFK76PQFNE (darkcoin.algo)

Developer Wallet 2: XQVJTVC7TAJ2SHQ7FDTD44UX2XYJNLNKATK3YBM2R2I5JVNKOGR4XDT4G4

Marketing & Development Wallet: 5QWEL3YRI4QA55BVTJYX6SACBULJPDI75SIG2YLC2T5LDOC3M7U5K3DTDQ

Liquidity Pool Wallet (Tinyman): GII6U3WIVUD5FTCGP3DG7IFTETBG5IPNFOFICKOYSYM42PYA5VN6N46E3Q

Liquidity Lock Wallet (80% supply via Tinylock through 5/31/23): MCXTHOHLWLBVMKUG2ERC5YOCUJ2BT2KSDXW3LBHSWDUFQCNJLETA4PQ7RU


# Dark Coin team

Anders Bergquist: Blockchain Developer (Full-Stack)

Non-ExistentDomain: Systems Administrator

Ragingdragon: Community Manager

Claude Baxter: Project Manager & ASA creator
ASA Creator Linkedin: https://www.linkedin.com/in/claude-baxter-787229114


# Dark Coin roadmap

Please be aware that dates listed may change based on unfolding circumstances. The dates listed below are simply goals we are setting to hold ourselves accountable in terms of creating a sense of urgency to accomplish these tasks.

Our main goal is to have a functioning closed beta produced within the next six months, by September 30, 2022. I am setting a wide margin as this will require partnering with other developers to achieve this.

   • 08/04/2022 it looks promising that we will meet this goal for the DAO dApp, though this date may need to be extended by a few weeks depending on how things play out. The privacy features are still in the very early stages. I would set expectations to have a functioning beta on testnet by Summer 2023.
    
This makes partnering with a developer one of the most critical and urgent tasks we must complete. I am focusing the majority of my efforts to achieve this, ideally I want to have formed this partnership by April 30, 2022, so that we can begin serious work toward the development of the closed beta.

   • 08/04/2022 Anders has joined the team! We are making solid progress toward the DAO voting app.
  
As our project grows, we will need to increase our moderation and marketing efforts. This will require bringing in members of the community as moderators on platforms such as Reddit, Discord, Twitter, and Facebook. Ideally we want the community to help select these individuals in the form of a vote. These individuals will help with the moderation of channels and assisting with communications. Ideally, we would like to accomplish this by May 31, 2022.

   • We have succeeded in expanding our team, and currently have sufficient manpower for moderation and marketing efforts.
  
We need to get Dark Coin and our icon listed across all major channels. This will be an ongoing effort as there are always new channels to apply for listings. For now, we are working to be listed on CoinMarketCap, Coingecko, Tinychart, and Algo Directory. Our teams goal is to be listed on all of these channels by May 31, 2022.

   • 8/4/2022 his is still an ongoing effort for most listing channels.
    
We need to achieve verification the Algorand Foundation and AlgoExplorer. For AlgoExplorer, it looks like we will not be able to receive verification until we have a functioning open beta of our DAPP. We are still learning the requirements for verification with the Algorand Foundation. For now, the deadline to accomplish this will be set for December 2022. This date may change as more information becomes available to our team.

   • We have achieved verification through Pera Wallet, but are still working to become verified by AlgoExplorer and the Algorand Foundation.
    
We are also in the process of applying for a grant from the Algorand Foundation. We are unsure what to expect in terms of requirements so will have to wait until we receive a response on Algorand regarding our application. Once we get an answer we will update the community and this document accordingly.

   • We have not been awarded any grant funds to utilize, though we have had positive communications with the Algorand Foundation and they are interested in Dark Coin, particularly the DAO functionality.
