
# Hexagon: a decentralized layer of governance on the Internet

**Abstract.** The first generation of cryptocurrencies gave us accessible finance in replacement of fiat currencies, which allowed cross border payments, cheap and easy payment processing, and freedom from seizure over decentralization. Yet not everything in the financial world became free and accessible. The second generation of blockchains with smart contracts tried to solve this issue by giving everyone an option to build their own decentralized programs, but it lacked scalability, a common set of rules and trust. Hexagon is the third generation of crypto breaking the barrier for businesses to raise money, users to save or invest and fairly receive goods, replacing traditional banking as a whole and classical regulators.

## The Beginning 

### 1.1 The dawn of the Internet 

The Internet is decentralized in a way that everyone can exchange information freely, there’s no certain rules of what data should be present. The only thing that Internet hardware controls is how to reach certain endpoints. Which means that the internet has no fundamental value, but rather a value of everyone who is connected. This increased global access to knowledge, entertainment, and communication. The Internet includes both traditional companies like post, shopping and ticket sales, and new companies like search engines, forums and e-mails. You can see that the new Internet companies only provide digital services processing data.  

People now can have more access to information about abstract subjects like science and politics, comparing different clothes and airlines, sharing or watching personally made content like vlogs, blogs or porn. Did we get rid of large corporations that control the market inside such a decentralized and globally accessible system? Unfortunately, the answer is no. Even new Internet companies have become dominant giants. At the time where everyone can launch their own website, we have examples like Amazon or Google, giving smaller sites no chance. I couldn’t think of any industry on the Internet including AI where we would have a market consisting of only small entities.  

Of course, the internet wouldn’t be possible without certain breakthroughs like copper and optic cables, powerful hardware, browsing software and routing, and data encoding protocols. Even though the internet is at scale decartelized, some centralization is needed like common protocols, address distributing and domain names of registration. 

There is no clarity of who is a subject for regulation on the internet. Humans themselves can be subject to their location’s country laws. Web servers can be located in another country. The company which owns these servers is registered somewhere else. And the domain registrar can be in a different location too. 

The Internet does not restrict anonymity; there are companies where you can buy or use a server or domain without revealing your identity. This gives us an opportunity to bypass tracking from ISPs by using tools such as the Tor Network. 

### 1.2 The dawn of blockchain  

Blockchains brought us to a new world where not a single entity or government has control over your money, and it is not physically stored only in one place. Keys to your wallets only exist digitally and therefore everyone can afford high security over them. To spend cryptocurrency, you only need an internet connection and the key itself, regardless of your location and identity.

This is only one function of money. Unfortunately, these days banks and private investors are responsible for loans to everyone who wants to get money for their business, and the relationship between public and companies is still controlled by the government, limiting them by bureaucracy, slow processing and therefore more restrictions. Blockchains too do not provide much trust and, like TLS and IP, only handle delivery and storage of data from one point to another, but they do not handle good relationships between entities on them. Traditional donations/fundraising are much more suitable for creators other than for running businesses, providing less transparency, flexibility, and control. That’s what Hexagon will be solving.

## 2. Key functions  of  Hexagon

### 2.1 Name system

Among all the internet layers DNS is perfect for our case, because IPs can be easily changed by moving domain’s resource records and lay too deep in the roots of the Internet functionality to manipulate, on the other hand data, information and computation is too heavy to move or copy, resulting to many scalability and decentralization problems today in other blockchain technologies.

DNS is a lightweight but yet very important system for binding users to apps or websites that process the data. Resolving them from the blockchain gives us all the necessary decentralization. Then we can split ownership over the names into pieces and whoever holds them has some control over this important part of a web app. For simplicity it’s  going to be called hex domains.

All sides are profiting from it. By selling the ownership app, builders can raise money or other resources without having any relationships with investors to the users who are willing to participate. Users trust those links with hex domains because what lays behind is not controlled by one entity, but rather ownership is split among all interested parties. Investors will have part of the direct control and not simple agreements on the paper and will immediately see true information about interactions and coin transactions of the app as part of what they want to buy.

Combining this with free and open-source software leads to great opportunities for developers, who today get no or minimum reward for their job, and to hex domain partial owners who will always have the required code to power the apps.

### 2.2 Transaction  details

Today transactions on the blockchains have only technical use, signifying over a funds transfer or a code call and are not used anywhere else. Hexagon’s goal is to put more useful meaning into transactions, recording the real name of the destination and the purpose into attached data. This idea has certain advantages and disadvantages.

First, when a developer wants to sell a hex domain over his app that processes coins, all the persons that would like to participate would see all the transactions associated with it, which gives them more confidence and therefore partial control over how funds are going, in case they are fake and sent by the hex domain’s seller themself.

Second, this data is provided by users that want to interact with an app or blockchain directly. They will have confidence that this information is immutable and associated with the desired receiver containing transfer details. This is going to help in case of disputes over received or not received goods.

On the other hand, it takes another piece from user’s anonymity, compared to other (pseudo) anonymous blockchains. Hexagon is going to  operate the same way without any verification of wallets. This is made to be a fair alternative with a purpose to bring more users from traditional finance, where all the personal data is given, and it lacks consumer protection because of bureaucracy. This is also attractive to traditional investors that can see real data that is impossible to modify or falsify and easily accessible without involving many institutions and long waiting time.

## 3. Blockchain  design

### 3.1 Acknowledgments

While Hexagon can be implemented on general purpose blockchains there are some limitations as following:

1.  Immutability of Ethereum smart contracts, but changes must be applied to the protocol not only to fixes and corrections, but to upgrading for more usage. On the other hand, Solana provides such a thing, but only in two ways where people still trust the underlying blockchain and contract code, without distribution of power and direct involvement.
    

2.  Transactions do not have any other mechanism to include data other than blobs. But hexagon requires a more sophisticated tag format with search functionality at least. This would require adding changes to the node code itself.
    

3.  To represent a control over each hex domain a new contract must be created with the same interface, while erc-1155 is not implemented by exchanges as “multi token”.
    

4.  Without running a full node other blockchains do not provide to users a sufficient level of decentralization to access data for example to resolve hex domains
    

Although using existing chains as an advantage provides access to liquidity,  from scratch we  must  build  wallets, local resolvers, governance, data stores and “scanners”.  So, a separate chain would be a better solution

### 3.2 Smart contracts

This part is also related to Acknowledgments.

Smart contracts were designed to create general purpose blockchains, where code is executed on many computers having properties like irreversibility, no third-party control over data and censorship resistance.

Unfortunately, it didn’t solve trust issues. In web2 you trust only the server you’re interacting with over the internet which runs your app, like Facebook. But smart contract blockchains add one or two other middlemen: the blockchain itself, like if you were running a node, and without a node you trust a third-party provider (MetaMask) or a site which lets you scan the blockchain (etherscan / bnbscan). And blockchain itself doesn’t give you any guarantees over safety of the smart contract code that you are calling, whether the address is wrong, or the code has malicious functionality.

Hexagon  tries  to  solve  this  issue  by  adding a layer  of  middleman  that  has  control  over  the  service  you  want to  interact  with, i.e.  hex  domains. This  also  solved  the  more  general  problem  of  free  software, where  users  can’t  review  over  the  whole  code  even  though  they  can. Those  middlemen  controlling  hex  domains  have  put  their  money  in  and  had  power  over  reviewing  the  underlying  service  in  order  of  its  good  functionality  and  growth  to  receive  profit  in  the  future.

### 3.3 Consensus

What we have seen in the first blockchains like bitcoin is that you can trust only the protocol, because it does not set the rules over data which will be produced by the network (input and output transitions) and limits the ability of participants to change those data so that you can only make new transitions. Consensus algorithms solve the problem of how you pay for the resources (like computation and storage).  

It’s hard to figure out how much block producers should actually earn and how much they should be paid for resources. On blockchains where block producers paid only by fees, you cannot have many transactions per second because fee revenue stops growing when you have many transactions. For example, when you add first 10 transactions you have $5 fees, but when you have 1000 transactions and add another 10 to them, you get much less fees. Computation increases O(n), but revenue is ~O(n^1/2). Therefore, on early bitcoin and PoS chains block producers are being paid extra (bailout), usually by minting new coins. Unfortunately, it’s very roughly calculated and highly exceeds how much is actually spent on computation.  

#### 3.3.1 Proof of Work

This first consensus protocol requires participants to add proof of work to interact with the network. When the network consists only of 100 users, everyone can participate in the consensus, where PoW plays the role of Ethernet in computer commination. Each participant has an equal chance of this block being added, and it’s chosen randomly over all participants.

This works only in the perfect world where resources are distributed equally and cannot be gathered in one place. Only  people with a lot of resources or an ability to aggregate them run such a blockchain. They play the role of middleman where your transactions can only be sent through them. But even in this case it still remains the way everyone can participate, without identifying themself. Over the competition every miner that adds new blocks still acts fair because otherwise it will not be accepted or replaced by other miners.

#### 3.3.2 Proof of Stake

Alternative consensus mechanisms like Ethereum need you to hold the chain's native coin and make a translation that submits your resources to run a validator. This is an example of a consensus where you should spend much more resources than you would have to pay for validator computation hardware itself. This means that your rewards are much less compared to what you spent (staked / frozen coins). Also, the network needs to pay much more for security, because the security protocol needs a lot of capital. This is approached by staking rewards in percents of your total stake. Because otherwise people with the money will move them from validator staking to other places with more attractable income rates. 

Another disadvantage is that the platform has control over new and existing validators, by controlling the coin value and flow, transaction mechanisms and policies over which they can only be withdrawn from staking. 

Also, what hexagon does differently is limiting the number of (full) nodes, therefore allowing users to verify the consensus by using software running locally without calling one trusted party. This solves the scalability issue so that the network would only have nodes that can afford more powerful hardware. Each validator knows who the current members of the consensus are and can provide clear data about it to the users. It also helps to solve communication problem where a lot of coins wasted because partisipants doesn't know how much they should pay for computation. 

#### 3.3.3 Governance

Compared to other blockchains, they have  governance either delegated to some other entity where miners/stakers have no decision-making  power, or it is decided by voting. In the first case (even if you have multiple clients) when you have a network split due to a disagreement, both sides get damaged, but the most popular side survives and takes almost all what this chain achieved from the beginning. For example, you can look at Ethereum vs Ethereum Classic or Bitcoin vs Litecoin. The opposition side is always very much smaller and not replacing the original chain with popularity or trust. Even when a network splits in two,  it’s  very hard to organize a dozen other different clients in the second alternative network to keep operating and have a sustainable user base.

Other blockchains governance voting is decided on their number of tokens, but when tokenomics is inflationary, they need to be stored at a place where you would have yield on them, usually it’s validator’s staking. 

Cryptocurrencies like bitcoin have no governance at all, which means they have no hard forks, and any version of the software can access the network.  This resulted in them keeping the same block size which left the protocol data structure untouchable. That’s why they have changed Satoshi's bitcoin view of it from a payment system to digital gold. And instead tried to develop L2 solutions like Lightning network that can be used for payments.  

Hexagon takes the second approach with on chain voting but takes it to the lower level where your vote decides on what client version you’re staying. Where after voting ends you decide on what version you stay organizing a separate chain with who made the same decision, i.e. auto fork. This would be impossible or very hard to make smart contracts or rollups if we didn’t have a separate chain.

### 3.4 Tokenomics

There are two types of tokenomics: limited supply and unlimited supply, though chains with limited supply sometimes have only 50% of all coins issued when another half is issued later at an unknown pace. While bitcoin’s inflation is only 0,8% and decreases by half every halving until it stops making new btc.

Hexagon will be using two economic principles. First, there’s a problem when a validator locks his coins; he can no longer spend them. This means that their value is lost to provide network security while decreasing usability. We add a mechanism of spending locked coins of validators by voting on proposals. This means validators are not wasting their economic activity and using it on network development, instead of spending it on themself. This also solves the problem of funding sources for the chain's purposes. But their coins will not be spent directly. When a validator joins, his balance would increase the vault balance and decrease it when he leaves. This would not affect validators' savings by keeping them neutral and decreasing conflict of interest.

Here comes the second economic principle. When validators use money from the vault, it increases total supply. But this would not affect anyone who’s participating in projects in a form of hex domains, because the value of their shares would only increase, making it easier to grow their projects and get more money for development.

Summarizing hex validators would be responsible for three forms of consensus:

1.  Automated  consensus  for  processing  average  transactions
    

2.  Spending from the vault for hexagon’s purposes
    

3.  Client upgrade voting
    

### 3.5 Accessibility

This chapter describes how users interact with the Hexagon blockchain.

As described earlier, average users can not verify consensus directly because it would take a lot of time and computation to download and validate all the blocks from the beginning even to check their balance. Hexagon will turn that into advantage by allowing users to call validators to get the current state and the list of validators that are left or joined. This would allow users to still have security and privacy without using one single party or having a powerful computer always validating the chain.

#### 3.5.1 Addresses

Today’s user experience consists of pasting creepy long byte addresses into their wallets that are hard to verify when they want to send money to someone. Hexagon would completely switch to using human readable names (e.g.  vitalik.eth), at as low cost as possible. In the past, destination addresses would represent public keys that a sending user would sign into a transaction. This is possible to switch fully to domains, because if a blockchain has domain -> pubkey table and the data is immutable it is secure to use them as destination addresses.

#### 3.5.2 Calls

The second scary thing for users is to constantly sign smart contract calls from their wallets that users have no clue what each call is doing. Today’s crypto wallets are dumb and cannot verify either the destination of money transaction or a smart contract call at least to be sure that such a destination wallet exists, and smart contract belongs to the open app page. Hexagon would build a verification framework of whether you’re sending a right transaction or not, this is much easier because many money flows would go through businesses backed by hex domains that want their records to look good, or otherwise those records would be inaccessible  to outside reviewers. Therefore transaction details have to be disclosed on chain.

#### 3.5.2 Transaction control

The third scary thing lying after the first and sometimes the second is the irreversibility of transactions. Today blockchains guarantee only the fact funds were sent or the code called, sometimes that’s even more scary than interacting with classical websites like Amazon, because behind classical websites are governments, shareholders, then executives and at the end customer support, that are far from perfect but together provide more protection to the users than average blockchain apps. On existing blockchains validators are only responsible for running nodes to keep the blockchain live and to stake coins to keep it secure, and on the other hand blockchain developers whose job is to grow or keep the same vaule of the coin so that validators wouldn't live and chain stopped working, but they are not restriced on other things they can do. Hexagon will provide clarity by identifying the purpose of each transaction, then adding hex domains to create inner consensus inside apps that would see user transactions flow without the need to control the running code directly, and they can make important decisions in case users are not satisfied about how the app works. And at the end validators of hexagon that have freedom and resources over decision making in various ways.

#### 3.5.3 Private keys

Third scary things is that the users responsible for their private keys themselves. In a case if you lose them you have no option to recover them. You need to store their copies in different places in case one will be lost. And today you can't set limit or additional checks on your actions (for example daily withdrawal limit) in case you keys are being stolen. There are options like account abstraction, where you can add your code to your on chain wallet, but you can end up in a trap when you can't change your own rules (if a hacker steals your keys equal to your identity). The second solution is to have a multisig family or close friends recovery, but this requires for them to also be users of your blockchain, otherwise they will act like walking backups for your keys. The third option is to have an organizations that could reset your key, fof example after verifying your email or phone number. On traditional blockchains there can be a ton of such organizations, which creates a trust issues. Hexagon solves this by building global optional framework for recovery and doing audit over it. 

#### 3.6 Focus

So many blockchains today are only focused on these metrics: speed, cost, storage, decentralization, and privacy. They are trying to compete for how many transactions they can process per second with N users on board. Along with transaction speed, they are decreasing costs like fees and costs for onchain storage. Also, they are trying to achieve higher decentralization and privacy over zk and sharding. With sharding you only increased number or participants, but you decrease how many entities you rely on to process your transaction and store your data. Zk can solve computational problems where you can rely on a single entity to process, releasing proof to everyone else. This scheme doesn’t work for data, because you need to store full not compressed data on as many computers as you can. A real-world example if zk can bring on board “billions of users”, Monero and Zcash have been released in the early era (later Tornado cash has been released on smart contract chains), but as time passed, they do not and never did dominate crypto market by any means, but still serve as reliable instruments.  

All these improvements don’t change basic principles of crypto like what it initially meant to be, should be for everyone, decentralized and anonyms, but don’t fix other fundamental problems. They promise that their blockchains can handle billions of users, but on the planet today there are 8 billion so only 8 blockchains could exist. Another problem would be that if we took any random 2 persons there’s an 80% chance they would be on different chains, so this would require such blockchains to be heavily connected. Such a system would be no different from the banking system that we have now. All around the world banks are connected at the same time being independent entities. Such a world would need competition not only on performance and numbers, but on how good your service you’re providing is. Hexagon is addressing this right now. 

## 4 Usage examples 

### 4.1 Monetizing open source 

You built a free and open-source self-hosted CRM system. Your repository has a lot of downloads and visitors because it pops up in google or GitHub search, and you want to monetize your work. Some common ways to do that are to add a donation banner on your front page or just a crypto wallet address, or you make your own paid hosting where you provide service for hosting a CRM for your users. 

There are some downturns in both of these methods. Donations usually provide small and unstable income; there's no way you could grow your project and do development full time. Making your own hosting needs a lot of resources like computing infrastructure, control panels, payment processing, landing site, and customer support. This approach involves a lot of corporate nasty behavior. First of all your users at first are being promoted with your own hosting other than an accessible way to setup it themselves, second users are charged overpriced because the price includes the cost of hardware (users may find a cheaper option for example aws instead of azure), costs for development (including domain, design, promo, etc.) and income for the project owner itself; third, users may have auto renewable subscription, additional non free services and extensions (like storage) and no option to migrate to their own hardware or backup recovery.  

How can Hexagon address this? A developer can get more money, because instead of a one-time donation, your users will have a concrete share of a future product. Collective development: you can easily delegate parts of your future product to other people but remain in a large share of control. Fair distribution: raised money will be in one place, and over them you can have a set of rules, e.g. a lock over time, or over product purchases. It will decrease greedy behavior because it will involve a portion of users. Transparency: users that only have a small share can view all the processes, and users that have not contributed yet or thought about contributing a lot will have more confidence over their opportunity to invest. Though to avoid fraud, the system needs to have a process, in which both parties will be confident about each other. This will be set by Hexagon globally but will open an endless number of opportunities for developers and investors.  

### 4.2 App market 

Today all the apps are being downloaded from App Store or Google Play. Both of these stores are controlled by corporations, even despite the fact that Android is an open system. They control how your apps are being accepted and rules for that. Even if you decide to install it from a file downloaded from another source, your android device will issue a warning. That means that your phone trusts apps that are signed from Google. It's well known that corporations control the distribution and revenue of your apps. There is an open-source version called F-Droid, which works like Linux packets, building your app from source, and keeping a list of all the apps.  

What Hexagon does differently, we create a decentralized infrastructure around this market, including financial infrastructure. This marked can include a direct Hexagon integration where control of those apps is distributed like hex domains. This would attract more developers because if an app has decentralized control over it, more people are willing to invest, and users who download such apps are more likely to trust the source. The market itself is governed in a decentralized way backed by Hexagon. This would mean a clear set of rules, a more friendly interface, and transparency. 

### 4.3 Refunds

You buy an API to get a weather forecast. This API is being sold to you by a number of requests or days. If this product is being sold to you on Hexagon, therefore the gateways for this API will be a hex domain resolved on the network. Also, if you buy it on the hexagon chain, your transaction will have your API user id, time of transaction, details about what API you bought and the amount of access you paid for (days, number of requests).  

After that you can interact with seller servers directly, without submitting anything on the chain. You can track how much recourses are left by exchanging digital signatures with the seller; you will mutually sign a message where it’s specified that you used N requests. Provider will wait until you sign a message with less requests left, and you will have his signed message where he guarantees that at least N requests are unused. If the seller does not receive your signature where you agree of less requests, he will stop providing API access to you. 

Hexagon will have an automatic refund functionality. Where the initial number of bought recourses is known with your payment transaction. Then you can submit a mutually signed message by the seller and you, where it says you used at least N, and get a refund for the rest. If the users submit a message for more money than really left, the seller replies with the message where you signed a less amount, and your refund will be blocked. 

This automated process is set by Hexagon globally and applied to any seller. This is better compared to other blockchains where the seller itself sets the rules for smart contract with your money, and these rules are not applied globally. For other chains, it’s almost impossible to implement it on a scale.  

You can get a refund in a traditional way. First you go to the seller itself, but his rules might not have a refund policy, or you will need to mail them a letter describing your situation and your bank account details, then wait for more than a week. If it does not work, the only option is felt to go to court with them, which is not accessible for almost all users. Your bank does not have the authority to transfer funds without the account owner's permit or a court order. Especially if you live in another country and buy your API access on the internet, you cannot access any government agencies where that business is registered, and it’s not suitable if your purchase wasn’t big enough.  

## 5 Infrastructure  

Not complete list of hexagon software and parties

- Wallets with the mandatory support of domains and trading. It should contain detailed transaction history and current cancellable subscriptions. 
- A platform where builders and companies can launch hex domains and see all available data. Also, the owners’ control panel. 
- Local clients for domain resolution and RPCs 
- Third party hex domain resolvers and RPC providers 
- SDK for builders to accept payments and required info to be put into transactions. 
- Node clients and proposals panel, along with oracles 
- Entities to giveaway wallet addresses and bridge with other chains

## 6 Summary

Hexagon stays as an alternative to the first and second generation blockchains. It enables better user experience and confidence, better validators and end users' participation in consensus, better environment for app owners to raise money and build scalable and user-friendly apps, more confidence for people wanting to invest their money in a secure and predictable way. First tier blockchains where one-coin chains, second tier are multi coin chains, we are taking an approach with token governance chain. This sounds more organic than an extensive growth approach taken by other new chains. Our goal is to create a trustworthy system in an industry which stands for “you should trust no one” and where the trust is often obscured.  
