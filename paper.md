
# Hexagon: a decentralized layer of ownership on the Internet

Abstract. The first generation of cryptocurrencies gave us accessible finance in replacement of fiat currencies, which allowed cross border payments, cheap and easy payment processing, and freedom from seizure over decentralization. Yet not everything in the financial world became free and accessible. The second generation of blockchains with smart contracts tried to solve this issue by giving everyone an option to build their own decentralized programs, but it lacked scalability, a common set of rules and trust. Hexagon is the third generation of crypto breaking the barrier for businesses to raise money, users to save or invest and fairly receive goods, replacing traditional banking as a whole and classical regulators.

## 1. Introduction

On the internet people use many websites, leaving personal information and assets, or using them to receive different kinds of information, buy things, or earn money to live their lives. But who do those sites belong to? Unfortunately, there are too many entities involved in control over it. First, owning IP addresses are not free and accessible for every man, they belong to both IANA, RIRs and ISPs. Before getting the IP, your PC resolves it from a domain name, rented from registrars who are also controlled by TLDs and IANA. Also,  almost everyone cannot have physical server hardware and rent it from hosting providers and cloud services.

All of those entities have control over site owners and users.  Also, humans themselves can be subject to their location’s country laws and laws of where his resources are located and where the company registered, all at the same time. Not in all cases law enforcement acts as it should, breaking the laws written for them or having too loose regulation due to lobbying or not working institutions.

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

What we have seen in the first blockchains like bitcoin is that you can trust only the protocol, because it does not set the rules over data which will be produced by the network (input and output transitions) and limits the ability of participants to change those data so that you can only make new transitions.

Their consensus protocol requires participants to add proof of work to interact with the network. When the network consists only of 100 users, everyone can participate in the consensus, where PoW plays the role of Ethernet in computer commination. Each participant has an equal chance of this block being added, and it’s chosen randomly over all participants.

This works only in the perfect world where resources are distributed equally and cannot be gathered in one place. Only  people with a lot of resources or an ability to aggregate them run such a blockchain. They play the role of middleman where your transactions can only be sent through them. But even in this case it still remains the way everyone can participate, without identifying themself. Over the competition every miner that adds new blocks acts fair because otherwise it will not be accepted or replaced by other miners.

Alternative consensus like Ethereum however need you to hold chain's native coin and make a translation that  submits your resources. That means the platform has control over new and existing validators, by controlling the coin value and flow, transaction mechanisms and policies over which they can only be withdrawn from staking. At the same time ASICs do not have constant price as well and are more volatile than GPUs, but while eth earns you 4% APY which would require ~17 years to have rewards equal to your stake amount, ASICs need ~2 years to cover the costs of buying them. And you don’t need anyone’s approval to buy or sell your ASICs.

Hexagon will be using a PoS mechanism to have economic functionality that will be described later. Each node on Hexagon has an auto upgrade mechanism (e.g. automated git), but what to pull is decided over coin voting. This removes the need for node operators to trust any third party and adds the second source of value to the coin.

Also, what hexagon does differently is limiting the number of (full) nodes, therefore allowing users to verify the consensus by using software running locally without calling one trusted party. This solves the scalability issue so that the network would only have nodes that can afford more powerful hardware. Each validator knows who the current members of the consensus are and can provide clear data about it to the users.

Compared to other blockchains, they have  governance either delegated to some other entity where miners/stakers have no decision-making  power, or it is decided by voting. In the first case (even if you have multiple clients) when you have a network split due to a disagreement, both sides get damaged, but the most popular side survives and takes almost all what this chain achieved from the beginning. For example, you can look at Ethereum vs Ethereum Classic or Bitcoin vs Litecoin. The opposition side is always very much smaller and not replacing the original chain with popularity or trust. Even when a network splits in two,  it’s  very hard to organize a dozen other different clients in the second alternative network to keep operating and have a sustainable user base.

Hexagon takes the second approach with on chain voting but takes it to the lower level where your vote decides on what client version you’re staying. Where after voting ends you decide on what version you stay organizing a separate chain with who made the same decision, i.e. auto fork. This would be impossible or very hard to make smart contracts or rollups if we didn’t have a separate chain.

### 3.4 Tokenomics

There are two types of tokenomics: limited supply and unlimited supply, though chains with limited supply sometimes have only 50% of all coins issued when another half is issued later at an unknown pace. While bitcoin’s inflation is only 0,8% and decreases by half every halving until it stops making new btc.

Hexagon will be using two economic principles. First, there’s a problem when a validator locks his coins; he can no longer spend them. This means that their value is lost to provide network security while decreasing usability (1.16Th/s asic = 0,08% vs 3eth = 0,0001% of the network, i.e.  you need to spend more money for the same security). We add a mechanism of spending locked coins of validators by voting on proposals. This means validators are not wasting their economic activity and using it on network development, instead of spending it on themself. This also solves the problem of funding sources for the chain's purposes. But their coins will not be spent directly. When a validator joins, his balance would increase the vault balance and decrease it when he leaves. This would not affect validators' savings by keeping them neutral and decreasing conflict of interest.

Here comes the second economic principle. When validators use money from the vault, it increases total supply. But this would not affect anyone who’s  participating in projects in a form of hex domains, because the value of their shares would only increase, making it easier to grow their projects and get more money for development.

Summarizing hex validators would be responsible for three forms of consensus:

1.  Automated  consensus  for  processing  average  transactions
    

2.  Spending from the vault for hexagon’s purposes
    

3.  Client upgrade voting
    

### 3.5 Accessibility

This chapter describes how users interact with the Hexagon blockchain.

As described earlier, average users can not verify consensus directly because it would take a lot of time and computation to download and validate all the blocks from the beginning even to check their balance. Hexagon will turn that into advantage by allowing users to call validators to get the current state and the list of validators that are left or joined. This would allow users to still have security and privacy without using one single party or having a powerful computer always validating the chain.

Today’s user experience consists of pasting creepy long byte addresses into their wallets that are hard to verify when they want to send money to someone. Hexagon would completely switch to using human readable names (e.g.  vitalik.eth), at as low cost as possible. In the past, destination addresses would represent public keys that a sending user would sign into a transaction. This is possible to switch fully to domains, because if a blockchain has domain -> pubkey table and the data is immutable it is secure to use them as destination addresses.

The second scary thing for users is to constantly sign smart contract calls from their wallets that users have no clue what each call is doing. Today’s crypto wallets are dumb and cannot verify either the destination of money transaction or a smart contract call at least to be sure that such a destination wallet exists, and smart contract belongs to the open app page. Hexagon would build a verification framework of whether you’re sending a right transaction or not, this is much easier because many money flows would go through businesses backed by hex domains that want their records to look good, or otherwise those records would be inaccessible  to outside reviewers. Therefore transaction details have to be disclosed on chain.

The third scary thing lying after the first and sometimes the second is the irreversibility of transactions. Today blockchains guarantee only the fact funds were sent or the code called, sometimes that’s even more scary than interacting with classical websites like Amazon, because behind classical websites are governments, shareholders, then executives and at the end customer support, that are far from perfect but together provide more protection to the users than average blockchain apps. On existing blockchains validators are only responsible for running nodes to keep the blockchain live and to stake coins to keep it secure, and on the other hand blockchain developers whose job is to grow or keep the same vaule of the coin so that validators wouldn't live and chain stopped working, but they are not restriced on other things they can do. Hexagon will provide clarity by identifying the purpose of each transaction, then adding hex domains to create inner consensus inside apps that would see user transactions flow without the need to control the running code directly, and they can make important decisions in case users are not satisfied about how the app works. And at the end validators of hexagon that have freedom and resources over decision making in various ways.

## 4 Usage examples 

### 4.1 Monetizing open source 

You built a free and open-source self-hosted CRM system. Your repository has a lot of downloads and visitors because it pops up in google or GitHub search, and you want to monetize your work. Some common ways to do that are to add a donation banner on your front page or just a crypto wallet address, or you make your own paid hosting where you provide service for hosting a CRM for your users. 

There are some downturns in both of these methods. Donations usually provide small and unstable income; there's no way you could grow your project and do development full time. Making your own hosting needs a lot of resources like computing infrastructure, control panels, payment processing, landing site, and customer support. This approach involves a lot of corporate nasty behavior. First of all your users at first are being promoted with your own hosting other than an accessible way to setup it themselves, second users are charged overpriced because the price includes the cost of hardware (users may find a cheaper option for example aws instead of azure), costs for development (including domain, design, promo, etc.) and income for the project owner itself; third, users may have auto renewable subscription, additional non free services and extensions (like storage) and no option to migrate to their own hardware or backup recovery.  

How can Hexagon address this? A developer can get more money, because instead of a one-time donation, your users will have a concrete share of a future product. Collective development: you can easily delegate parts of your future product to other people but remain in a large share of control. Fair distribution: raised money will be in one place, and over them you can have a set of rules, e.g. a lock over time, or over product purchases. It will decrease greedy behavior because it will involve a portion of users. Transparency: users that only have a small share can view all the processes, and users that have not contributed yet or thought about contributing a lot will have more confidence over their opportunity to invest. Though to avoid fraud, the system needs to have a process, in which both parties will be confident about each other. This will be set by Hexagon globally but will open an endless number of opportunities for developers and investors.  

### 4.2 App market 

Today all the apps are being downloaded from App Store or Google Play. Both of these stores are controlled by corporations, even despite the fact that Android is an open system. They control how your apps are being accepted and rules for that. Even if you decide to install it from a file downloaded from another source, your android device will issue a warning. That means that your phone trusts apps that are signed from Google. It's well known that corporations control the distribution and revenue of your apps. There is an open-source version called F-Droid, which works like Linux packets, building your app from source, and keeping a list of all the apps.  

What Hexagon does differently, we create a decentralized infrastructure around this market, including financial infrastructure. This marked can include a direct Hexagon integration where control of those apps is distributed like hex domains. This would attract more developers because if an app has decentralized control over it, more people are willing to invest, and users who download such apps are more likely to trust the source. The market itself is governed in a decentralized way backed by Hexagon. This would mean a clear set of rules, a more friendly interface, and transparency. 


## 5 Summary

Hexagon stays as an alternative to the first and second generation blockchains. It enables better user experience and confidence, better validators and end users' participation in consensus, better environment for app owners to raise money and build scalable and user-friendly apps, more confidence for people wanting to invest their money in a secure and predictable way.
