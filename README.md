<p align="center">
  <img src="https://blockterms.com/blockterms.png" width="225px;">
</p>

<h1 align="center">Whitepaper</h1>

<p align="center">
  <a href="https://blockterms.com">blockterms: Collective Structures for Digital Currency</a>.
</p>

<p align="center">
  <a href="https://github.com/blockterms/whitepaper/releases">
    <img src="https://img.shields.io/github/release/blockterms/whitepaper.svg?style=flat">
  </a>
</p>

## Contents

- [Terminology](#terminology)
    - [Digital Assets](#digital-assets)
    - [Blockchain](#blockchain)
    - [Distributed Ledger Technology](#distributed-ledger-technology)
- [Introduction](#introduction)
- [Partnership Address](#partnership-address)
- [Common types of Partnerships](#common-types-of-partnerships)
- [Ownership Structure](#ownership-structure)
- [Settlement Algorithm](#settlement-algorithm)
- [Transaction Attributes](#transaction-attributes)
- [Partnership Economy](#partnership-economy)
- [Ownership of Partnership Address](#ownership-of-partnership-address)
- [Settlement Frequency](#settlement-frequency)
- [Accrual of smaller amounts](#accrual-of-smaller-amounts)


## Terminology

#### Digital Assets

"Digital Assets" are also called "crypto coins", "crypto tokens", "crypto currency," 
"virtual currency", or "digital currency". Most of these assets are based on cryptographic protocol 
of a computer network that may be centralized or decentralized and closed or open-source.

In this paper, Digital assets represent assets that are used as a medium of exchange and/or a store of value.

Popular examples of digital assets are bitcoin, ether, miota, neo and ripple among many others. As of 2018, there are 
over 1300 known crypto currencies. All of the assets issued by these currencies are considered 
Digital assets.

Concepts used in this whitepaper can easily be applied to nation state currencies like dollar, 
renminbi or yen when used in the context of online transfers. The transaction fees and the 
regulation around handling traditional currencies might be prohibitively expensive.

>https://en.wikipedia.org/wiki/List_of_cryptocurrencies

#### Blockchain

From [wikipedia](https://en.wikipedia.org/wiki/Blockchain).

A blockchain is a continuously growing list of records, called blocks, which are linked and secured 
using cryptography. Each block typically contains a cryptographic hash of the previous block, a 
timestamp and transaction data. By design, a blockchain is inherently resistant to modification of 
the data. It is "an open, distributed ledger that can record transactions between two parties 
efficiently and in a verifiable and permanent way". For use as a distributed ledger, a blockchain 
is typically managed by a peer-to-peer network collectively adhering to a protocol for validating 
new blocks. Once recorded, the data in any given block cannot be altered retroactively without 
the alteration of all subsequent blocks, which requires collusion of the network majority.

blockchains are secure by design.

#### Distributed Ledger Technology

Distributed Ledger Technology or (DLT) is a digital system for recording transaction of assets. 
Details of these transactions are recorded in geographically distributed multiple locations at the 
same time. Distributed ledgers do not have a central data store or a central authority that 
controls the contents of the data store. blockchain is one implementation of Distributed ledger 
technology.


## Introduction

**blockterms: Collective Structures for Digital Currency**

blockterms enables multiple parties to form a digital currency payment address and define 
an ownership structure for how to settle funds in that address and how often. Consumers pay 
at the payment address in exchange for goods and services and all the parties involved in the 
ownership structure get their appropriate value of the transaction or transactions.

To provide an example from gig economy, a community ride sharing app "AirLift" and individual 
driver can be partners on blockchain or distributed ledger via blockterms. These two partners can 
agree upon their ownership structure depending on the most common implementable terms defined as 
follows. 
	
1. Driver gets 70% and AirLift gets 30% of the consumer payment transaction.	
2. If it is late at night, driver should be rewarded 10% more.	
3. If the driver has a good reputation, AirLift wants to reward the driver with an extra flat fee per 
ride up to 1000$ per month.
	
As you can see, the terms could be very simple and could get very complex.

There are two important parts in the above partnership example.

1. Ownership structure.  
2. Settlement Algorithm. 

Ownership structure determines the participants and their share of value in the incoming transaction/s  
depending on agreed terms and conditions. Ownership structures can be public or private, stored privately
or on public/private distributed ledger. 

Settlement Algorithm executes the terms and ensures the partners get their share of the partnership. 
Settlement algorithms can be open sourced or closed.


## Partnership Address

Partnership addresses are generated for a given currency. A visual representation for a public partnership 
address can be obtained going to url 

> https://blockterms.com/partnership/[address].svg?size="small|medium|large"


The visual representation of a sample address with both flat fees and percentage partnership looks as follows.


![Bitcoin Partnership Address](images/btcprtnaddress.svg)
  

bitcoin is the currency of exchange for this partnership. The dotted area indicates flat fees and each 
color represents different partner and their percentage ownership. estb 2018 indicates this partnership 
was established on blockchain since the year 2018

This image visual can be linked to from different marketing material for the product or service offered 
at this partnership address.
 
## Common types of Partnerships

#### Flat Fees Partnership per transaction  

A flat fees is paid to the partner per transaction. If the value in the transaction is greater than the 
flat fees, the flat fees is ignored.

|Parameter|Description|
|:----|:----|
|fees|A flat fees is paid to the partner per transaction.|
  

#### Flat Fees Partnership per transaction with limits

  A flat fee is paid to the partner per transaction with a maximum upper limit set per day or per 
  week or per month etc or a overall upper limit.
  
|Parameter|Description|
|:----|:----|
|fees|A flat fees is paid to the partner per transaction.|
|timely_limit|Depends on timely_frequency. If the total flat fee paid to this partner reaches this limit during the time_frequency duration. The flat fee will not be paid for the remainder of the timely_frequency duration.|
|timely_frequency|daily, weekly, monthly, every N days|
|max_upper_limit|This is the total maximum amount that will ever be transferred to this partner. After that point the partnership ends.|
  
#### Percentage Partnership per transaction
   
   A percentage of the transaction amount will be paid to the partner. Sum of all percentages should add up to 100%
  
|Parameter|Description|
|:----|:----|
|percentage|A percentage of the transaction amount will be paid to the partner.|


#### Percentage Partnership per transaction with limits

A percentage of transaction is paid to the partner per transaction with a maximum upper limit set per 
day or per week or per month etc.


|Parameter|Description|
|:----|:----|
|percentage|A percentage of the transaction amount will be paid to the partner.|
|timely_limit|Depends on timely_frequency. If the total amount paid to this partner reaches this limit during the time_frequency duration.  No more amount will be transferred for the remainder of the timely_frequency duration.|
|timely_frequency|daily, weekly, monthly, every N days|
|max_upper_limit|This is the total maximum amount that will ever be transferred to this partner. After that point the partnership ends.|

Once this percentage partnership ends, proportional increase for other percentage partners or this funds get collected to specific addresses.

#### Time Varying Flat Fees Partnership

  In a Time varying flat fees partnership, the fees increases or decreases depending on a 
  simple/compound interest rate. This partnership can have timely limits or overall limit. 
  Timely limits stop after reaching an upper limit during a time period where as the partnership 
  ends when the over all limit is reached. 

   This kind of partnership is a good candidate to raise investment or funding for short term projects.

#### Time Varying Percentage Partnership

  Similar to above. Instead of flat fees, partner gets a percentage of transaction.

#### Runtime partnerships

  Runtime Partnerships depend on runtime information available in every transaction in transaction 
  attributes. Settlement algorithms parse the transaction attributes to make dynamic decision on the ownership 
  share of each partner.

#### Complex Partnerships

   Complex partnerships depend on external data like performance of partners for the duration of 
   settlement.

## Ownership Structure

Ownership structure of a partnership could range from simple to complex. For public partnerships, this 
information is stored on public blockchain. Current reference implementation uses NEO.

Data Stored on blockchain for simple partnerships

```
1. Address where the payment is accepted
2. Currency of the Contract
3. FlatFeestructure addr:val,addr:val......
4. PartnershipStructure addr:val,addr:val......
5. A Website Address where users can find more information
```

The format of the data could be slightly different depending on the underlying blockchain capabilities. The data should 
be serializable to json or xml very easily. Consistency and standardization of this format is very important to make blockterms 
information on the blockchain interoperable with other emerging systems in distributed ledger technology space.

For slightly more complex ownership structures, the data structure would also involve conditional statements as parameters.

## Settlement Algorithm

Every partnership address pairs with a settlement algorithm which executes the terms of the partnership.
It should be possible to standardize settlement algorithms for most common use cases and allow 
advanced users to define specific algorithms for special cases.
 
Settlement algorithms could be open source or private, simple or complex.

Settlement is a zero sum activity. All the incoming funds have 100% destination.

Simpler settlement systems depend on fewer parameters, and the amount of data the settlement system 
depends on determines its complexity.

Some examples of simpler systems are.

* A book author partners with a website/mobile app to sell their new book at a flat fee based partnership. 
This also applies to other kinds of products promoted on websites/television media like games, apps, 
movies, manufactured products.
* A small investor can partner with an artist/craftsman to upfront some investment in exchange for a 
time limited percentage partnership on sales of the creative work.
* A partnership of a small team with cross sectional skills. e.g., a group of skilled professionals 
could agree on a percentage terms for a small project they do together like a documentary crew or 
a volunteer medical team or short term advertising campaigners etc.
	
In all these cases, the terms of partnership are relatively simple and depend on fewer parameters. If there are 
funds in the partnership address, the account will be settled according to the pre determined terms. 

In some other cases, runtime parameters are sent as part of the transaction using extra information in 
the transaction via transaction attributes. The extra information could be simple name value pairs like cookies
or http parameters.  

In certain complex use cases of real world scenarios, instead of moving the data near a settlement algorithm, it would be
lot easier to move the settlement algorithm near the data.

Some examples of such complex systems are

* How to fairly distribute funds among members of a winning football team?. 
* How to fairly distribute funds among contributing members of an open source software/hardware/design project?
* How to fairly distribute funds among a support team based on number of tickets closed?
* How to fairly distribute funds among a social network community members based on their reach for a 
messaging campaign?

In all the above cases, it might be hard to come to an agreement on what is fair. The amount of data 
collected and the importance of data to the context of the settlement determines the complexity and 
feasibility of an implementable settlement system.

![Settlement System](images/settlement.svg)

## Transaction Attributes

Transaction Attributes can be sent along with a payment transaction. This extra information is used 
by settlement algorithms to execute the terms of partnership which need context data to make decisions.

Transaction Attributes will be part of the blockchian or distributed ledger. Clients that do not want this 
information public can send encrypted transaction attributes using shared keys.

ECDH enables two parties, each with their own private and public key pair can generate a common shared key to be able 
to send and receive encrypted messages.

The payment sender makes an api call by passing a public key to a partnership address end point and 
get a shared key. Messages sent with this shared key between two parties can be decrypted only by 
these two parties.

>https://en.wikipedia.org/wiki/Elliptic-curve_Diffie%E2%80%93Hellman

## Partnership Economy

Blockchain is often described as internet of value. Blockterms leverages the potential of blockchain 
to deliver a digital partnership economy.

A group of individual addresses can form a partnership address and a group of individual addresses and or
partnership addresses can form other partnerships thus forming complex chain like and pyramid like structures 
of cooperation to provide goods and services in marketplace. This is analogous to a group of atoms forming molecules 
and a group of atoms and or molecules forming other molecules. 

A variety of complex chains and pyramids are possible with payment addresses inside other payment addresses 
and so on. All of these structures can be linked together using urls to these addresses in webpages.

![Atoms](images/atoms.svg)

![Molecules](images/molecules.svg)

Pyramid is a bad word to use in finance but these digital sky scrappers allow us to inspect pricing of 
common goods and services offered in the market place and debug for what components can be improved to 
reduce prices and make price efficient economic modules.

![Modules](images/module.svg)

## Ownership of Partnership Address

Who ever owns the edittoken, owns the access to edit the partnership. The keys to the partnership 
address are owned by blockterms. These keys are only used to sign transactions offline and submitted to 
the currency network. 

edittoken is generated and created when the partnership address is created. edittoken is optionally linked 
to email address. If a user forgets the edittoken a link to reset the edittoken is sent to the email address. 

It may be possible to build a multi signature system where multiple partners have to signoff to make a 
change in the partnership information. This will eliminate the need for edittokens.


## Settlement Frequency

The minimum is block level. Everytime a new block is created for the currency, that block is inspected 
for partnership addresses and the transactions are settled.

At the other end is manual. The funds accumulate until someone with valid edittoken for the partnership 
manually calls for settlement of funds. This option is very helpful to preview the settlement before 
actually transferring funds.

In currencies that do not have blocks it may be possible to have a transaction level settlement.

## Accrual of smaller amounts

After every settlement, if the share of a partner is below a very small threshold value, these amounts 
are accrued in the partnership address and transfer of the funds are withheld until their sum adds up to 
a value above the threshold value. This is also true for settlement fees. 

We batch multiple of these small amounts into one transaction. The threshold value is different for different 
currencies
