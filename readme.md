>> ![img](https://i.imgur.com/vOCwOan.jpg)

> >>>>>>>RAHUL GORAI
> 
>>>>>>> TEAM - Neptune
> 
>>>>>>> Sabre Hack 2019
>>>>>>> 



**Sabre Hack**


**Neptune - BaaS (  BaaS)- Blockchain as a Service for Aviation
D-App **


**Introduction **

**1. Blockchain and Aviation**

Blockchain is one of the technology that has been identified as one of the technologies that may have a major impact on the future of aviation. It can. Be compared to the evolution of cloud and private infrastructure. They way cloud is an inevitable technology that has to be there for any business models to grow and success, blockchain can’t also be ignored.

Aviation being a class of critical technology where every logs, data, experience and pipeline matters the most is one of the brightest areas of blockchain application. They way blockchain can serialise the aviation strategy and process is commendable. 

**2. Abstract**

The blockchain technology has stepped into a phase in which it has gained more maturity and its benefits and use cases are becoming clear. Aviation is one of its use case where this technology is being leveraged on a high scale. The use of smart contracts and tokenisation with digital asset management can predominantly change the way Aviation processes.

The tech world is one of the most dynamic segments of this universe. For the one moment everyone is behind technology and the next moment the technology becomes obsolete. Each day a new framework and technology is released but still, there needs to be something which should have the power to carry the mass together. D-Apps are the decentralised way of communicating to each other using mobile and web applications. In this time of world, where data becomes crucial part of any human being , we can’t risk to give it to any central authority to govern and control. D-Apps solves this problem, here you hold your data and you are the sole person to make it secure using your cryptographic keys. Proof of work is one of the most important feature of blockchain, this tells us that what ever you do in your business is recorded and stored in blockchain. So if you are a musician and you play guitar and publish your music in the blockchain network, it’s always yours. The proof fo work algorithm of Ethereum preserves your work. Neptune is also built using the similar ideologies of D-Apps. It is true that in today’s time its impossible to completely decentralised something but we can still tend towards maximum decentralisation.

Neptune is a Blockchain as a Service which has been built on Ethereum and Libra blockchain to leverage the features of core blockchain technology to Aviation process and business. On top of this as a service model, Neptune- DAPP is a web +mobile application which uses Neptune’s core APIs to give and user interface to operate the tasks.

More parts of Neptune services are discussed in later sections.


![Imgur](https://imgur.com/tLayu2Q.png)


**3. QuickStart Guide**

**Neptune Blockchain as a Service.**

NBaaS is a model to offer blockchain layered services for Aviation processes. In Neptune the services are divided in 4 main pillars of Aviation industry. 


**1. Security **

Security is one of the major part of Aviation industry. Be it a simple way of security check-in or a complex algorithm running on the microprocessors of the IOT devices, security is an inevitable part of any Airport. Neptune provides following service for security.


**A. Neptune - Security**

This is used to connect to the Xray IOT devices to the Neptune API endpoint which will proceed by sending the logs to the Blockchain network and attach the identity to the block created. This keeps track of security logs of each individual and each genesis block which is the first on generated form the flyers first experience is connected to the next block.


![img](https://i.imgur.com/jsMf3Nq.png)

The security lot emits the logs of each individual and a block gets created. After that the identity of the individual is attached to the block and the block is pushed to the chain after it gets mined. The transactional data get stored in the wallet who’s copy resides in a DB in Google Cloud Platform.

**B.  Neptune- Baggage**

This service is for baggage tracking which can be connected to the boarding process of Aviation. Once the flyer is boarded through the D-App and its physical baggage is deposited, its information gets logged to the blockchain. Again as above, all the blocks gets connected to the genesis block of the flyer’s first flying experience.


**2. Bookings and payments**

**A. Neptune-bookings**

This is booking API of Neptune. This uses Libra blockchain to create a decentralised environment to connect the users/flyers to the airlines directly. This removes the middlemen and hence reduces the cost. There is no broker charges or convenience charges. All you need to do is to connect to this API and book. 

In Neptune, Web application is provided which is connected to the above API.

**B. Neptune - Wallet**

Wallet is one of the essential feature of any blockchain product. Any transaction which happens through the blockchain is via Wallet. In Neptune, a non-deterministic wallet is provided which is created by the combination of public and private keys of the user. This wallet is connected to the blockchain network. Any flow of information which happens through it is recorded in the wallet.

“Read on a blockchain is free but write costs gas”

**C. Neptune - Loyalty**

Loyal claims to be reinventing the creation, reward and management of customer incentives. It envisages to allow the extension of the partner network while also reducing the cost associated with reconciliation and settlement. Furthermore it claims to allow the expansion of marketing capabilities by enabling personalised offerings with real-time insights.

**3. Pilot **

**A. Neptune-pilot-logging**

This service is for the Aviation safety. In the initial case we record the pilot logs and patterns in a blockchain. Any negated block creates an anomaly and calls for a manual verification.

![img](https://i.imgur.com/8WacyZc.png)

In Neptune pilot logging API the service is attached to the cockpit logs of the pilot window. All the traces which is normal as well as abnormal is tracked in the blockchain. Each of the activity block is associated with an identity of the pilot and as soon as a negated block (a block describing an abnormal situation) is created in the blockchain, an anomaly is raised.


**4. Architecture of Neptune**

In terms of open-source Neptune uses public permission as well as permission-less blockchain. The prior one is a private network where only the authorised people will be able to view the ledger even on the peer to peer network and the later one is public blockchain where Neptune uses public network. 

In Neptune , for private blockchain it uses Ethereum and ETH currency and for the public blockchain it uses Libra blockchain. 

**A. Service segregation **

![img](https://i.imgur.com/aIPDehO.png)


**C. The peer to peer network**

Neptune’s peer to peer model works very similar to other Ethereum based decentralised applications. Each instance which runs on top of the Ethereum framework runs individually on each devices which tends to use this application. Since there is no central server, none of the instance is relied on it. The machine which uses it has all the source code. Once any transaction takes places , which means any step in Neptune , example user registration, it updates the ledgers on every node of the network.
Here we don’t rely on any central system controlling and governing everything. This satisfies the first and the foremost law of the blockchain ecosystem. Let’s deep dive more into this network.
Neptune web app is basically an angular based application with a backend of python and node. This needs a server to run, and as stated we don’t have any central server in this model we assume that the machine which runs this application has all the dependencies installed, or more precisely a docker based platform to run the app.

* Database - All the transactions which happens around the application are stored in the Ethereum blockchain as a package of blocks which are linked together. Let’s take and example - Assume someone placed an order using Neptune platform and after few days cancelled it and asked for a refund, then all these steps will be recorded in the blockchain ledgers and shared to everyone. Hence this becomes tamper less. Ethereum uses and algorithm of proof of work to ensure the integrity of data pushed into the blockchain.

* The Algorithm and Code- So where does all the code base resides ? So first of all, every login in Neptune is written in Solidity in the form of Smart Contracts. The buy, sell , refund, dispute etc is a specific smart contract individually. Each one of them is deployed in Ethereum Virtual Machine, it converts the code into Ethereum byte code and then deploys it into the ethereum blockchain.

![img](https://i.imgur.com/P4IbnpU.jpg)

**C. The model**

Here, the model of Neptune’s architecture is discussed in terms of top view, where the three main parts of the application is shown, one is the front-end which is the end users tab, the backend APIs, the ether payment gateway called as metamask and the EVM (Ethereum Virtual Machine). Later we will discuss about its core event transactional model.

**Top View**

* The Decentralisation

When we talk about decentralisation of any distributed application, we need to understand that we cannot isolate the application from the world to make it decentralised. Rather we divide the application into many parts and then make the core decentralised. Core refers to the parts where the logics of blockchain resides. The goal is to fetch maximum decentralisation, not complete decentralisation.

* Frontend 

The frontend of Neptune is build on Angular 7 with all the source code packaged into modules. This is hosted on a central server which connects users to its backend using Python APIs. These APIs are capable of connecting to the Ethereum network which is completely decentralised.

* Backend

The backend consists of the wrapper APIs connected to Solidity smart contracts to connect to public nodes and finally runs on ethereum virtual machine.

* Wallet

Metamask is a bridge that is used to connect the application to ethereum public network. Neptune web uses metamask chrome extension and the mobile app uses metamask mobile client.

![](https://imgur.com/KMp7jTe.jpg)

**D. Neptune’s Transactional Model**

* The Transaction

In Neptune transaction is referred to each step which takes place in lieu of ethers. A transaction is defined as a service which this application provides in turn of some amount of ethers. A profile creation is a transaction which will have some ether value, an advertisement is a transaction and a dispute management service is also a transaction in Neptune.

* Crypto Identity

In Neptune , Metamask is used as a crypto wallet which uses public and private key to generate tokens to push any transaction to the blockchain network. The private key gives you an identity and one can only act on behalf on this. This is always stored in your local machine which never goes online making no one able to control the identity except the owner. With the combination of the private and the public key one can perform any allowed action on the centralised and de-centralised network. This means Neptune stores all of your transactions and actions cryptographically secured so that nothing is tampered.
So as it has been already stated that due to limitations of scalability in networks we combine different approaches to achieve maximum decentralisation. Neptune uses both, decentralisation and some part of centralisation. Both plays a vital role in the architecture of Neptune. This is explained in the below topics.

* Backend

From technical point of view, there has to be a bridge that connects the smart contracts to the web/mobile applications. In today’s fully de-centralised applications, where the clients interacts with smart contracts directly the bridge is narrowed down to JSON RPC API capabilities of public APIs , which in turn are forced to exist because of the fact that not every device can run and support its individual network node.

There can be two major interaction in a decentralised network.

* Listening to the network events (like token transfers) / reading the network state.
* Publishing transactions- invoking state-changing smart contract functions like token transfer.



![](https://imgur.com/nmWVcJ0.jpg)

In Neptune from the backend point of view these happens-

* We listen to a particular network event by continuously polling the network.
* Once we get an event, we perform some business logic and then decide to publish a transaction in response.
* Prior to publishing the transaction, we want to ensure that it will likely be mined (in Ethereum, the successful transaction gas estimation means there are no errors against the current network state). However, we can’t guarantee that the transaction will be mined successfully.
* Using a private key, we sign and publish the transaction. In Ethereum we also have to determine the gas price and gas limit of the transaction.
* After publishing the transaction, we continuously poll the network for its status.
* If it takes too long and we can’t get the status of the transaction, we have to re-publish it or trigger a “fail scenario”. * * * Transactions can be lost for various reasons: network congestion, dropping peers, network load increase, etc. In Ethereum, you can also consider re-signing a transaction with a different (actual) gas price.
* After we finally get our transaction mined, we can perform more business logic if needed. For example, we can notify other back end services about the fact of the transaction being completed. Also, consider waiting for a couple of confirmations prior to making final decisions regarding the transaction.

![](https://imgur.com/zSmIOyw.jpg)

* Publishing Transactions

Steps:

* Preparing the transaction. Along with transaction data, this step implies requesting the network state in order to find out whether this transaction is valid and is going to be mined (gas estimation in Ethereum) and the transaction’s sequential number (nonce in Ethereum).

* Signing the transaction. This step implies the usage of the private key. Most likely, here you’ll want to embed the custom private key assembly solution.

* Publishing and republishing the transaction. One of the key points here is that your published transaction always has a chance to get lost or dropped from the de-centralised network. For example, in Ethereum, the published transaction can be dropped if the network’s gas price suddenly increases. In this case, you have to republish the transaction. Moreover, you may want to republish the transaction with other parameters (at least with higher gas price) in order to get it mined as soon as possible. Thus, republishing the transaction can imply re-signing it, if the replacement transaction wasn’t pre-signed before (with different parameters).

![](https://imgur.com/cwphs9o.jpg)

Using the above reproach in Neptune we determine the transactional system. This is explained below.
The user executes a function in a smart contract, which ultimately allows the back end to perform a successful charge transaction.

* A back end service responsible for a particular task listens to the event of charge allowance and publishes a charge transaction.

* Once the charge transaction is mined, this back end service responsible for a particular task receives an event from the Ethereum network and performs some logic (including setting the next charge date).


**E. Technical Architecture**


1. The Central Part | In terms of technical architecture, as Neptune comes in two variants, one as a web application and other as a mobile application to serve the purpose on every kind of available devices. The former is built on Angular 7 and the mobile version is built using React native. Both of them are packaged as an image on a docker container and hosted on Google cloud platform. Further , these front ends are connected to the decentralised part using python wrappers. The local data is stored in MongoDB which sometimes serves as a local cache. In some cases where you want data fetching speed to be high and can’t rely on block-chain network Neptune uses its local DB to make processing faster. Further, these wrappers are connected using RabbitMQ messaging services which works on a publish-subscribe fashion. These web hooks provide an asynchronous connection of the front end of Neptune and the blockchain network. All these wrapper services, local database and messaging queues resides under Amazon EC2 instance. 2. The Decentralised Part | Until now, all the technical dependencies were hosted on Google cloud or AWS, which is completely centralised. The decentralised part contains Ganache-Truffle-Web3.js framework which allows the central part to connect to the decentralised world. Ganache is a in memory blockchain which provides test ethers to develop any application. In current scope of Neptune, Ganache is used as a blockchain network. Web3.js is a very powerful javascript library which allows any javascript based framework to connect to Ethereum blockchain. Neptune is based on Web3 and Truffle. For the core part, which is smart contracts Neptune uses Solidity.


![](https://imgur.com/4ZNIkvA.jpg)

**F.  System Architecture**

The system architecture extends the technical architecture and explains how Neptune interacts with the lower layers of its decentralised services. The Neptune’s package is connected to the public blockchain layer using Web3.js library wrapped by python APIs. This combines together to bring up the communication between the nodes …. Node1 to Node n. These nodes resides on the Ganache local arena for the scope of the this application.

![](https://imgur.com/WWGy0kw.jpg)

**G. Neptune Data Flow Diagram**

In Neptune the data flow depends on the services we use. Typically there are four service which generates data following nested services. So each time the user uses Neptune it generates data , a block gets created and the public ledgers get updated for all. Once the block is ready it depends on the gas value to mine the block and chain it to the blockchain.


![](https://imgur.com/Lr6SKfs.jpg)

**G. TECHNICAL DOC**

![](https://imgur.com/CBkK8Go.jpg)



