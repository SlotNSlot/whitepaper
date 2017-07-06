# Table of Contents
* * *
#### 1. Introduction
#### 2. Market Analysis
##### 2.1 Market Size
##### 2.2 Typical Market Problem
##### 2.3 Ethereum Solution
#### 3. SlotNSlot Platform
##### 3.1 Make or Play
##### 3.2 Multi Platform
##### 3.3 Send Emoji
##### 3.4 Fair & Transparent
##### 3.5 Low Cost
#### 4. Game Design
#### 5. Pseudo Random Number Generator (PRNG)
##### 5.1 Motivation
##### 5.2 Prior Attempts
##### 5.3 SlotNSlot Solution
#### 6. Team 
#### 7. Business Model
#### 8. SlotNSlot Token (SLT)
#### 9. Crowdsale (TBD)
#### Appendix

* * *

# 1. Introduction

Online gambling has experienced great leaps recently that has never been observed before. A huge portion of revenues in the market comes from video slot machines, leaving significant market potentials if tran\sferred to a better platform. Traditional slot game platforms, offline casinos or online video slot machines, provided players with limited choices, little information about games, and a great burden and risk of one-directional trust.

SlotNSlot aims to provide an ever-lasting, trustless, autonomous gambling platform with extremely low operation cost, where anyone in the globe can both make and play amazingly fun and incredible slot machines. With the aid of rising Ethereum world computer, the platform achieves fast and economical designs. The games are perfectly fair and transparent with a trustworthy implementation of Random Number Generator, and users can enjoy both on the web with PCs and on mobile devices. SlotNSlot platform also gives users a variety of choices with the games settings, which never had been possible in traditional markets. The experience is made further exciting with a feature of communicating through Emojis between users.

Random numbers are genetated using seeds from participants to keep fairness. The exchange of this seeds between users and smart contracts takes place in a semi-p2p channel on Ethereum, Whisper, with a commit&reveal protocol to ensure there's no fraud. Unlike traditional games where the play window is determined to calculate the result, SlotNSlot game system determines the game result to inverse-calculate the play window, which is just as fair and same as the other way around, still with a huge decrease in the cost and speed of the operation.

This paper is to explain what and how SlotNSlot plans to do in detail, to achieve such goals. The team and its basic guidelines in developing the platform and the project itself is addressed. SlotNSlot platform will open a everlasting arena of slot games and change the paradigm of gambling, while representing how a project on developing a decentralized application should look like. The project will evolve eternally with the dedication of the team, community, and users all around the globe.

* * *

# 2. Market Analysis

### 2.1 Market Size

Global gambling market is steadily growing. Especially, its online counterpart is increasing rapidly, leading the whole market growth. From 2006 to 2010, global gambling market showed 5% of compound annual growth rate(CAGR), while it was estimated to increase to 10% during 2011~2015. This doubling of growth rate is surely due to the growth of online gambling market.

Online gambling market volume was 37.91B USD in 2015, and is forecasted to grow with approximated 9.5% of CAGR until 2020. With high penetration of network access and mobile devices worldwide, the market will grow further if a trustful and enjoyable service was introduced. The fact that users are free of burdens and risks of carrying cash would boost it much more. SlotNSlot on top of Ethereum technology will play a major role in this rise.

<img src="https://s3.amazonaws.com/slot-n-slot-whitepaper/onlineGamblingMarketGrowth.png" style="max-width: 100%; height: auto;">

As an example of gambling on Ethereum, a simple “dice” gambling service had 12,718 ETH user winnings with more than 50,000 bets over 1 year of service. They offers several dices with different win rates, from 5% to 90%. If players bet uniformly among those dices, which is actually the case at the time of writing, the house earning is at least 8-fold of that winnings, which is more than 90,000ETHs. This is a revenue equivalent of 23.4M USD. (260 USD/ETH, as of July 1st 2017)

Another similar service that launched its beta on June 2017, had roughly 3,000 bets with 2500 ETH user winnings. Though the estimated revenue couldn’t be obtained due to its dynamic win rates and payout modified by the service provider, a simple projection over one year with a conservative assumption that it will neither grow nor diminish still gives 30,000 ETHs, which is 7.8M USD. (260 USD/ETH, as of July 1st 2017)

On top of these market estimates, SlotNSlot is estimated to profit a minimum of 10,000 ETH on its beta release in Q4 2017. This estimate is still quite conservative since i) Slot machines are much more enjoyable and popular than simple dices, ii) SlotNSlot is a multiple-role platform where anyone can make and/or play slot games, and iii) SlotNSlot beta release is scheduled to support both Web and Android. The team is and will be dedicated to developing a suitable service to realize the estimates, or even better results.

### 2.2 Typical Market Problem

Traditional online gambles, as well as offline ones, provide a one-way service where the only one thing that users could do is to put their money in the machines and trigger spin, or nothing. This one-way service is valid only when users fully trust the service provider. In other words, users were playing on slots believing, or hoping, that the service providers not be a fraud. This one-directional trust causes several problems. The service providers might vanish with all user deposits, especially when it’s provided in a country where online casinos are illegal. In some occasions, service providers deny to give out deposits on users with extremely high payouts.

A major problem with the one-way trust of traditional gambling services is that there’s no confidence that they’re using a proper Random Number Generator(RNG). A proper RNG is key to the fairness of a gamble, since gambling should be understood as ‘equally unpredictable’ game to every single party of the table. Traditional gambling services typically doesn’t provide any information about their RNG, or even if they did there’s no way to assure that they’re telling the truth.

Another huge imbalance of traditional gambling is the information asymmetry. Because they are centralized IT services with a central server, the service providers have access to a vast amount of information on user activities, enabling modification of services dynamically. On the other hand, typical piece of information offered to users on slot games is usually a pay table. Some regions might legally force casinos to provide their probability accounting reports(PARs), but this still leaves a significant barrier to the information due to its complicated procedures.
On a relatively broader scope, there’s also an asymmetry on the choice of roles. For ordinary people, running a online casino, or even a single slot machine, is merely impossible since it’s rather a form of business which requires related knowledge, programming, operations on online service business, and most of all, a significant amount of bankroll. Thus, a single option of choice for most people is to decide whether they want to get into a blackbox set by those bankers, and play an unbalanced game.

Traditional online services expose another weak point. An online service with a central server might suffer unstability. If the back-end server experiences failure, the service also fails at the same time. Service upgrades or regular maintenance would also temporarily suspend the service.

### 2.3 Ethereum Solution

<img src="https://s3.amazonaws.com/slot-n-slot-whitepaper/decentralize.png" style="max-width: 100%; height: auto;">

All of the problems suffered by traditional online gambles mentioned above will be relieved with Ethereum. Because the Ethereum blockchain is sustained by countless nodes around the world, a service on it is perfectly **fail-proof**. Service protocol updates can be done immediately and there’s no need for maintenance in blockchain-based server.

Ethereum blockchain **reduces the cost** of service significantly. SlotNSlot utilizes this to enable anyone to operate own slots without a large amount of bankroll. Any ordinary user of SlotNSlot can own a slot game with a few amount of ETH.

Every transaction on Ethereum blockchain is copied and recorded in all of the nodes in the chain. It’s perfectly **transparent** and **trustworthy**. Furthermore, the team will always make any relevant source codes open to the public. This would offer a perfect access to information on SlotNSlot. Regardless of choice of roles, i.e. slot bankers or players, anyone can access them without any limitation, even someone not using the service can do.

Lastly and most importantly, SlotNSlot uses a Pseudo Random Number Generator(PRNG) designed to run on Ethereum blockchain. This PRNG would generate a random number that is **equally unpredictable** to participants. Both slot owners and players can be ensured that the games are always fair. More details about PRNG are to be dealt in later section.

* * *

# 3. SlotNSlot Platform

### 3.1 Make or Play

SlotNSlot is a platform that offers easy slot mechine creation for users who want to be a slot banker, and slots list with enough information for others who want to play. Unlike traditional online casinos, people in SlotNSlot have a chance to decide whether they will be a slot banker or just play slots others make. They may have a strategic option and make a strategic decision to win the game after considering their budget, slots list and etc. SlotNSlot team believe that this will bring a brand new pradigm to the scene.

Slot bankers are to determine some parameters of their slot machines to reap the most out of them, while generating the best experience for players visiting them. The most basic numbers to be determined are the total stake of ETH to wager on the specific machine(_totalStake_), and minimum/maximum bets allowed(_min_/_maxBet_). 

Holding an decent amount of credit on the slot, i.e. _totalStake_, is important since relatively low credits would run out quickly and close the slot, meaning the banker would possibly lose over the slot. This is also affected by the size of maxBet allowed. In short, bankers will struggle to find a proper level of _totalStake-to-maxBet ratio_ such that their slots don’t run out of credit in a short term period.

Bankers have control over hit frequency(_hitFreq_) and maximum payout(_maxPay_) as well. _hitFreq_ refers to the rate of paylines that gives any payout to the player, _maxPay_ the size of the biggest payout on a payline. A high value in _hitFreq_ might appeal to the players, though too high a value could disadvantage banker’s profitability.

As users create a slot with designated parameters, a probability matrix of the whole paytable is determined and uploaded in a new contract on the blockchain. To ensure that neither bankers nor players are significantly expected to win on the long-term, Return To Player(RTP) is always kept between 90 to 110 %. The exact value of resulting RTP won’t be offered to users, but if anyone wanted an exact RTP it can be calculated from the paytable contained in the contract, yet a complicated computation.

After creating slots, bankers can enter one of the slots owned, and watch others play it. While watching a player on the slot, they can send Emoji to the player to express their emotion. If they don’t feel like watching their own slots, they can visit and play on other’s slots.

Players on SlotNSlot, on the other hand, are fully confident of what they’re doing. Unlike traditional slot machines, slots in this platform always notify sufficient information to players. Hit frequencies, maximum payout and the banker's balance are always visible to players. They can determine their own choices, which slot to play, how much to bet, how many lines to play, and when to quit playing. Winning or losing depends strongly on the strategy and luck.

Players will choose a slot to play considering the slot settings. After entering a designated slot session, they will determine _amountBet_, the number of credits to bet each payline, and _numLines_, the number of paylines to play each spin. These value of _amountBet_ is, of course, in the range [_minBet_, _maxBet_].
The actual amount of credit bet each spin, _spinBet_, is the product of _amountBet_ and _numLines_.

> _spinBet_ = _amountBet * numLines_

At beta launch, SlotNSlot games will provide 20 paylines. Players can choose a number among 1~20. If a player made a spin with _numLines_ = 5, then the paylines 1, 2, 3, 4, and 5 will be selected for the game. The figure below shows current design of 20 paylines in SlotNSlot, which is widely used for online slot games.

<img src="https://s3.amazonaws.com/slot-n-slot-whitepaper/win-line.png" style="max-width: 100%; height: auto;">

Note that _hitFreq_ is defined as the rate of spins that give any payout to the player, which calculates over each payline the same way. This makes the slot to have more frequent payouts with more paylines because there exists a chance of coinciding hits for multiple paylines. For one spin, the probability of giving any payout looks like below formula.

> _probability_ =  1 - (1 - _hitFreq_)<sup>(_numLines_)</sup>

Players can utilize never-seen-before strategies in SlotNSlot. A simple example of such strategy is to play on slots with the lowest balance. Some players may find it more fascinating to play in slots with higher hit rates. This freedom of choice is available because the platform gives detailed information about slots, which was not offered in traditional gambling markets.

### 3.2 Multi Platform

Much of online services are mobile dominant in recent days. SlotNSlot team is currently developing clients for both HTML5-based web and Android, and iOS will be supported soon enough. At the time of writing(as of July 1st 2017), there is no mobile slot games application running on Ethereum network. SlotNSlot team aims to develop a prototype and release the beta on Google Play Store in mid July, which will be the world first mobile slot game running on Ethereum network.

For the support of mobile application, the team is developing two major solutions. One is to accelerate Ethereum light node synchronization and transaction(contract) deployments. The other is to control possible issues caused by unstable network connections on mobile devices. SlotNSlot team will do the best to resolve these issues, and you will see the results on Google Play and AppStore, soon.

<img src="https://s3.amazonaws.com/slot-n-slot-whitepaper/multi-platform.png" style="max-width: 100%; height: auto;">

### 3.3 Send Emoji

One of the key features of SlotNSlot is the communication between users via Emojis. Example of such feature can be found in one-on-one arena video games such as _Clash Royale_ or _Hearthstone_. The team expects such quick expression of emotions between users will make far more exciting user experiences in SlotNSlot.

Bankers and players can send Emoji at certain situations to express their emtions to their opponent. It is expected that users will actively use Emojis when they're in extreme sentiments. e.g. out of anger that they lost a huge bet, or joy that they got a decent prize. Sending Emoji is a paid feature, which usually activates when players get huge prizes or the opponent gets bankrupt. Costs paid to send Emoji are transferred to the platform’s public wallet and distributed to token holders periodically. This will make up a significant portion of profit in SlotNSlot business model.

### 3.4 Fair & Transparent

With Ethereum network and smart contracts in its backend, every single information on SlotNSlot cannot be hidden from anyone, from slot settings and balances to every play history. When players visit slots, the parameters set on them are all visible, so players can always know what they are doing.

Games in SlotNSlot are provably fair due to its PRNG. Being provably fair on a gambling table means to have a well defined PRNG. A well defined PRNG would give out random numbers that are equally unpredictable to both participants, namely bankers and players. Detailed information about PRNG is to be explained in later section.

Play histories and remaining balances are always available to both bankers and players. For those who are more knowledgeable about computer programs, all source codes for SlotNSlot service are recorded on Github repositories. The team will always keep recent updates with every information channels. 

### 3.5 Low Cost

While storing all play histories on blockchain, the games are played partially off-chain, utilizing a semi-p2p communication protocol between the banker and the player. Games are played and recorded with minimum on-chain transactions, thus reducing the cost significantly.
	
Unlike traditional “platform” businesses, SlotNSlot has no middleman. The platform owns itself. The transaction fee collected is also distributed to token holders. Both parties, i.e. bankers and players, can utilize the platform with extremely low cost, and if they hold some tokens, the cost might be reduced further, to a near-zero level.

* * *

# 4. Game Design

Unlike usual slot machines, SlotNSlot game doesn’t have a pre-determined reel strips. Instead, it holds the paytable and the probability table and utilizes the seeds sent from the banker and the player to put into the PRNG and generates random numbers. Game results are determined on mappings between these random numbers and the paytable. This design is mathematically equivalent to the typical slot game design. SlotNSlot uses this design to extremely decrease the gas price required to do the computations.

The team is currently working on both possibilities, i.e. typical and new design. At the time of service launch, either one of them will be selected depending on the gas price required to run each design. In this description, the latter design will be briefly explained, and for the typical reel strip method design and mathematical probabilities, refer to the Appendix at the end of document.
 
SlotNSlot game logic is as follows
 1. A banker creates a slot with slot_parameters. The paytable and probability matrix is created with those parameters, which are then stored in a new contract representing the slot session.
 2. A player enters the slot session, and make a spin with spin_parameters, which are sent to the slot session contract with PRNG seeds from both users.
 3. Slot session contract creates random numbers, records the random numbers and relevant payout results in its internal storage, and sends the same data to the player’s client.
 4. The client shows a result screen corresponding to the payout. If there are multiple cases, any one of them are chosen randomly. This randomness doesn’t need to be unpredictable since it doesn’t affect the slot game itself, i.e. the result is already determined.
> Note that this logic doesn’t explain about the logic for PRNG.
 
_The team is aware of some possible issues implementing this logic. The issues and team’s current response is as follows._

* Multiple payline spins

	* Unlike typical design, SlotNSlot’s logic doesn’t take into account the coinciding wins, and considers a multiple payline spin as a sequence of independent single payline spins. A player making multiple payline spin is not to modify the probability of results but to quickly iterate multiple spins over time. A mathematical explanation of this issue is included in Appendix.

* Different result screens on banker and player

	* Though it might feel strange to have different result screens, it still doesn’t affect neither the fairness nor the result of the game. The logic is still preferred due to its extremely low gas consumption. A detailed description about the algorithm to generate the result screen is included in Appendix.

_The team is open to any debates in any channel for improving the service. If you have any concerns and suggestions about the service, please contact the team with Github, Twitter, Hipchat or any other communication channels._

* * *

# 5. Pseudo Random Number Generator (PRNG)

### 5.1 Motivation

The main goal of PRNG design for SlotNSlot is to ensure “equal unpredictability” to both parties of the game, while keeping a fast response and low cost of transaction fee. In traditional designs where a central server generated and provided the random number, RNG was done by taking a mean of entropy, or “a seed” from the server. Implementing this design on smart contracts depends on the entity who commits the code, thus making it difficult to be used in a deterministic virtual machine. In this section, several prior implementations are described, and then the design used in SlotNSlot.

### 5.2 Prior Attempts

One typical way to obtain a pseudorandom number from blockchain is to utilize the data in certain block, such as blockhash or timestamp. This method has been discussed for long, and it is well known that the miners have a chance of manipulating the odds. This is even a serious problem when the miner of the transaction generating the random number is either of slot participants.

RANDAO has developed a collective commit&reveal solution where some number of participants pledge certain amount of bounty and get rewarded if they honestly act in generating a random number, otherwise losing the pledge. This method has some limitations to be implemented for SlotNSlot. It requires a sufficient number of participants which may slow down the response and raise the cost due to the need for reward. Moreover, this is vulnerable to DDoS attacks, endangering the entire system.

Dao.Casino implemented a per-transaction strategy. A pair of private and public key is generated by an banker and the public key is stored in the contract. Then a random number is sent from the player and encrypted by the banker. The contract then verifies the encrypted public key with the existing one, and generates the random number. This implementation uses numerous transactions for each bet, affecting both the response and cost.

iDice utilized an intermediary between blockchain and an external RNG service, Oraclize. This also requires a number of transactions between the game contract and the Oraclize contract, thus having a high dependency on blockchain confirmation time and cost. Furthermore, this solution is not a provably fair one since an external service cannot be ensured to be honest.

FunFair solved much of these issues by implementing a state channel design, which enables unlimited number of iterations off-chain with only the initiating and finalizing of the channel requires an on-chain interaction. The weak point here is that the results aren’t recorded on-chain in realtime, and exception handling comes as a serious problem, e.g. when either of participants suddenly disconnects from the channel.

### 5.3 SlotNSlot Solution

SlotNSlot deploys a semi-p2p PRNG using the Whisper protocol in Ethereum with all those prior challenges in consideration, which is achieved in following order.

 1. [p2p] A player triggers a spin in the slot, calling the banker to send his own encrypted random number N’ (= SHA3(N)) with Whisper protocol.

 2. [txn] The player generates his own encrypted random number M’ (=SHA3(M)) which isn’t used previously, and send it to the game contract with N’.

 3. [txn] The game contract id is sent to player.

 4. [p2p] Player sends his M’ with game contract id to the banker to verify the game.

 5. [p2p] The banker verifies the game, and sends his original N to the player.

 6. [txn] The player sends both the original numbers (N, M) to the game contract. The contract verifies (N, M), uses XOR(N,M) as a seed to generate the random numbers, and records the result.

<img src="https://s3.amazonaws.com/slot-n-slot-whitepaper/randomNumberGenerator.png" style="max-width: 100%; height: auto;">

In this design, both bankers and players check the fairness on-chain, while relieving much of the blockchain dependency using the semi-p2p method, _Whisper protocol_. At the same time, game results are recorded on-chain in atomic units, making the exception handling much easier.
Although this implementation has relieved some of the prior challenges of RNGs on blockchain, it still suffers some intrinsic limitations, i.e. minimum transactions required. The team will consistently keep its efforts in developing a better design of RNG.

* * *

# 6. Team 

The team is currently working in a country where legislation on cryptocurrencies is not built. The country strictly bans online gambling with any currencies considered as valuable, domestic or global. Though a legislation doesn’t exist yet, the team still desires to avoid any means of legal issues in the region. For the time being, no exact identification of any team member will be revealed. The team sincerely appreciate generous understanding.

Instead of posting personal information, the team will validate credibility by source codes and open communications on the web. The team would appreciate and diligently participate in any means of debates, questions, corrections, requests, and feedbacks on the relevant communication channels. Currently this will include the team’s Github, Twitter, and Hipchat. With the concept of Decentralized Autonomous Organization(DAO) in mind, the team’s major role is believed to be developing core smart contracts to build a decentralized application. The platform will then run on an autonomous consensus between token holders.

The team currently consists of 7 developers with degrees in Computer Science and Electronic Engineering, on top of years of experience in relevant fields, 1 UI/UX designer with great skills and experience, and 2 project managers who are serial entrepreneurs as well. The team works in a decent work environment where it can make quick responses and decisions while operating the tasks efficiently.

* * *

# 7. Business Model

The major sources of profit are expected to be  
* % fees from slot games, and  
* fees paid to send Emojis.  

> A detailed business model is to be determined soon.

* * *

# 8. SlotNSlot Token (SLT)

SLT token is solely for dividend yields. Any profits made on SlotNSlot platform will be cumulated in its public wallet, and distributed token holders in proportion to the amount they hold. Total number of tokens will be fixed at the very first issuance and ever. Major guides are as follows.

- The team still must possess at least 10% of the total amount issued, to encourage the team for better engagement.
- Every use of funds raised from crowdsale should be inscribed with a specified purpose.
- In determining the details of crowdsale, embrace as much suggestions from the communities as possible

> the details of SLT and its crowdsale will be updated soon

* * *

# 9. Crowdsale (TBD)

* * *

# Appendix

This part of documentation is to help understand the in-depth principles of SlotNSlot games, with brief comparison on traditional slot games. The explanations include arithmetic and algorithmic notations. For those who are solely concerned about business aspects of SlotNSlot, this part can be skipped.

### A. Traditional games

SlotNSlot games have 5 virtual reels, each arranging three symbols in the play window. The play window, thus, has a 3X5 (rowsXcolumns) symbols matrix. Traditional games have a predetermined “reelstrip” for each of those 5 virtual reels, where a reelstrip is a fixed length of permutation of the game symbols with replacement. The proportion of each symbol in a reelstrip is the key to the metrics of games.

These reels stop at a position determined by the RNG running on the back of the game. Here, for the i-th reel, the probability of a symbol s to stop at the designated payline position is n<sub>s</sub>(i)/l(i), where n<sub>s</sub>(i) is the number of symbol s on the i-th reelstrip, and l(i) is the total numer of symbols on the i-th reelstrip, i.e. the length of the reelstrip. A payout is determined after all of these 5 reels have stopped at certain positions.

p<sub>s</sub>(i) = n<sub>s</sub>(i)/l(i)

Typically, a paytable is defined as a mapping between numbers of prizes and some number of repeated symbols from the leftmost reel on a payline. This number of repeated symbols required to win a payline is typically from three to five. The probability of a win of k repeated symbols s on a payline can be calculated recursively. 

prob<sub>s</sub>(5) = Π<sub>(i=1 to 5)</sub>p<sub>s</sub>(i)

prob<sub>s</sub>(k) = Π<sub>(i=1 to k)</sub>p<sub>s</sub>(i) - Σ<sub>i=k+1 to n</sub>prob<sub>s</sub>(i) 

_where prob<sub>s</sub>(k) refers to probability of k repeated symbols s from leftmost reels, prize<sub>s</sub>(k) refers to the prize multiplier of k repeated symbols s from leftmost reels_

Then, the expected RTP is the product sum of those prizes and probabilities over every symbol, expressed in percentage.

RTP = 100 * Σ<sub>(s∈symbolset)</sub>Σ<sub>(k=3 to 5)</sub>prob<sub>s</sub>(k)*prize<sub>s</sub>(k)

_*note that iteration omits k=1,2 since there’s no prize for 1 or 2 repeated symbols, i.e. prize<sub>s</sub>(k)=0 for k=1,2_

If we assume that there is only one payline in the game, defining all individual proportions of symbols on each reel, i.e. defining p<sub>s</sub>(i), is mathematically equivalent to defining winning probabilities, i.e. prob<sub>s</sub>(k), in line with the result of the former way. Seeing a five-K win, i.e. prize<sub>K</sub>(5), with a probability of 0.01% is just as same as getting a specified number out of a dice having numbers from 1 to 10000, which is what traditional video slots are actually doing.

However, in real life most slot games are played with multiple paylines. Multiple paylines games are far different from above assumptions and calculations. Paylines affect each other depending on how reelstrips are designed. Suppose there was no sequence of symbols A and K in the first reelstrip, and the symbol A had stopped in the middle of the first reel. Then there would be no winning paylines with symbol K in the same play window. In short, multiple paylines have a complicated dependency on one another.

Even with an extreme assumption that the reelstrip is not defined in advance, i.e. each of three symbols in the first reel is chosen independently, paylines are still dependent on each other. On a 3X5 play window, the maximum number of paylines that are fully independent of each other is 3. Thus, playing a spin with more than 3 paylines make the calculation of probabilities much more difficult.

On top of that, if unusual winning conditions such as featured games and scatter symbols are added to the game, the calculation is merely checking all possible outcomes of the 3X5 play windows. If all of 5 reelstrips had a length of 100, the iteration would be 10<sup>10</sup> possible outcomes (10 billions), with every iteration checking 3X5 window for winning conditions. This is even worse when reelstrips are not defined, where the total iteration would be the number of distinct symbols in the game to the power of 15 (number of cells in 3X5 window). For a game with 10 symbols that is 10<sup>15</sup> iterations. (a quadrillion)
> Scatter symbols are winning conditions such that if a specified number of that symbols are scattered on any position of 3X5 play window then it’s considered a win. Prize is usually featured games, e.g. free spins.
 
Each iteration in those billions or quadrillions leads to even more computations since typical 8 to 10 symbols games have complex winning conditions mentioned above. If any of those iterations led to featured games, the payout for that iteration needs to be calculated recursively. The practice is to get the expected RTP with a simulation.
 
### B. Design of game system and PRNG

In the traditional game designs described above, each stopping positions of 5 reels is determined by RNGs. Because there is no way to get a pure RNG on the Ethereum blockchain, SlotNSlot obtains a PRNG with seeds from each of two participants. This process of PRNG is run on a smart contract on the Ethereum blockchain, and the game results are determined by the random numbers generated.

In designing the structure of game logic, contracts, and PRNG, the team’s top considerations were as follows.
- It must take less than 10 seconds to get a game result on the user client after the user hit the spin button. (i.e. 360 spins/hour)
- The gas fee required for each spin must be minimized
- The result of a game must be determined on the game contract.

The lower bound for game speed is set to be 360 spins/hr (i.e. upper bound of 10 seconds for each spin) since traditional mechanical slot machines mostly did better than this. PRNG couldn’t be built with Oraclize.it or RANDAO, since they both required a minimum waiting time equivalent to the blocktime on Ethereum.

SlotNSlot design utilizes a message call to the game contract with seeds from each participant to get the fastest response with game results, which is confirmed to be less than 10 seconds in current Ethereum testnet.

The team has considered two possible designs of contract structures, i) one that generates random numbers to decide stopping positions for each of five reels and calculates the result inside the contract, which is equivalent to traditional slot games, ii) the other where random numbers are generated on top of a mapping to probabilities for payout amounts.

i) When a banker requests to create a slot game with (_hitFreq_, _maxPay_), a random permutation of predefined reelstrip is generated, and a game contract is created with the permuted reelstrip and paytable stored in its internal storage. When a player visits and makes a spin, random numbers are generated to determine stop positions for five reels, and the resulting 3X5 symbols and payouts are calculated in the contract and sent to the player client. This would seriously increase the number of computations required, thus the gas fee. Furthermore, the RTP of the game changes depending on the permutation of reelstrips, so the parameters of the game not only determine the proportion of symbols on reels but also set some constraints on the arrangement of symbols on the reelstrips. Keeping these constraints when creating reelstrips further complicates the computation. This can be partially avoided by making a predetermined set of reelstrips and using them without permutations. Players might feel tedious from seeing repeated payout windows, still with complex computations required inside the contract.
 
ii) A banker creates a slot game with (_hitFreq_, _maxPay_), then a game contract is created with a corresponding table of mapping between prize amounts and their probabilities. In this case, random numbers are mapped to a certain prize amount in proportion to its probability. (e.g. if a prize of 500 credits has probability of 0.01%, then 0.01% of the random number range maps to the 500 credit prize. If this probability was the minimum, then the range would be 1 to 10000, and only one specific number out of 10000 would be mapped to 500 credit prize) Implementing this design needed a new definition of a multi-line game. Traditional multiple payline games had different probabilities and RTP with regard to paylines played. Here, we define a multi-line game as repetition of independent single payline games. A game with N paylines is equivalent to repeating a single payline game N times. In this way, RTP is always kept at the same level. This implementation of “accelerating the game speed with multiple paylines” seemed, to the team, quite reasonable and fair to both participants of the slot game as long as all the information was open public and the RNG was provably fair. Following is the flow of the game.
 1. A banker creates a game. A game contract is created with a prize table corresponding to the slot_parameters stored inside.
 2. A player makes a spin. The bet amount and number of paylines are sent to the game contract with the seeds from the banker and the player.
 3. The contract creates random numbers corresponding to the number of paylines played, and the result is calculated with the prize table and the bet amount. All of them are sent to the player client.(banker receives same data if monitoring the play)
 4. The client calculates an appropriate 3X5 result window corresponding to the prize.

Next section describes some possible issues, solutions, and details of the implementation.

### C. SlotNSlot Implementation

In traditional slot game, a paytable is a mapping between winning conditions and their winning prizes, i.e. multipliers. In SlotNSlot implementation, a prize table is a mapping between winning prizes and their probabilities. Any paytables in traditional designs can be transformed into prize tables if the probabilities of winning conditions are calculated “deterministically.” (But this is not the case because in traditional games winning conditions take place with different probabilities regarding the paylines played.) Thus, in SlotNSlot design, prize tables are constructed by determining a specified probability on each prize amount. Then, the sum of all probabilities on prizes except for zero prize is equal to the _hitFreq_.

If a player made a spin with 20 paylines, 20 random numbers would be generated, each corresponding to a winning prize and its probability. Suppose the result was 15 lines of 50 credit and 5 lines of 100 credit. (This is still a very unlikely event since 20 lines all paying out has a probability of roughly 1/10<sup>14</sup> for a game with _hitFreq_=0.2) Then the client would try to plot 15 paylines with the winning condition of 50 credit, and 5 paylines of 100 credit. This is obviously impossible if the symbols of both winning conditions are distinct. This simple but highly unlikely example shows that there exist some combinations of prizes which cannot be expressed on a 3X5 window.

To solve this problem, SlotNSlot client sums up all the resulting prize amounts, and then finds a combination complying to the sum by searching from the largest prize amount in the prize table. With the example above, the client adds all the prizes to get 1250 credit, and then finds the largest prize amount that is smaller than 1250. This would result in a window with a 1000 credit line and a 250 credit line. In other words, the prize amounts in the prize table must be designed in such way to produce no result of unplottable combination.

A huge barrier to this design is that, because of a long range of numbers on prize amounts, it is merely impossible to create such prize table that has “no” unplottable combination at all. The probability of having those unplottable combinations would be negligibly small, but still it must be known how small the probability is, and there must be a way to ensure there is no other unplottable combinations with higher odds.

The team has come up with an alternative way to find a proper prize table design. With some simple guides, a prize table is created under some constraints given by slot parameters. Map this prize table to the paytable, and run the prize-table-to-game-result plotting simulation, with 20 paylines. If the simulation passes a specified number of iterations, use the prize table for the slot parameters. Otherwise, modify some values in the prize table. Following is the order of the process.

* step 1: Set RTPs on every (_hitFreq_, _maxPay_) combination.
	* Refer to next section for determination of RTP
　　
* step 2: Generate a prize table {prize(i):prob(i), for i=0 to k}. A simple guide is to make k relatively small. This requires some prize(i)’s to map to multiple winning conditions on paytable. Keep the prize table under the constraint(_hitFreq_, _maxPay_, RTP).
	* this was done by using an Excel sheet
   
* Step 3: Map the prize table to the paytable, and run a simulation of 20 paylines game over 10<sup>N</sup> iterations.
	* Step 3.1: If the simulation finds an unplottable combination before 10<sup>N</sup> iterations and its probability from the prize table is greater than 1/10<sup>N</sup>, return to step 2 and adjust some values.  
	* Step 3.2: If the simulation stopped with an unplottable combination of a probability smaller than 1/10<sup>N</sup>, run the simulation again.  
	* Step 3.3: If the simulation succeeds to iterate 10<sup>N</sup> times, use the prize table for that (_hitFreq_, _maxPay_, RTP).
　　
 * Step 4: Repeat steps 2-3 for every (_hitFreq_, _maxPay_, RTP) combination.
 
where constraint(_hitFreq_, _maxPay_, RTP) is  
prize(k) = _maxPay_  
prize(0) = 0  
p(0) = 1 - _hitFreq_  
Σ<sub>(i=1 to k)</sub>prob(i) = _hitFreq_  
Σ<sub>(i=0 to k)</sub>(prize(k)*prob(k)) = RTP(_hitFreq_, _maxPay_)  
prize(i) < prize(j), prob(i) > prob(j) for i<j  
 
In actual game implementation, if clients ended in a situation where they got a prize with a probability smaller than 1/10<sup>N</sup>, i.e. an unplottable combination, the game would pop up a special featured game where a random-alike animation would finally show the actual prize won. This is still highly unlikely to happen, and is considered yet fair enough since the prize is given out anyway.
 
### D. _hitFreq_, _maxPay_, and RTP

Though all information is available on SlotNSlot, the resulting RTP of slot parameters (_hitFreq_, _maxPay_) won’t be notified on the game clients. It is fully users’ choice to look at the documentations and source codes to find out the exact RTP of every combination, or to infer it from the levels of parameters they choose. To help users predict RTPs with those parameters, but not so exactly, RTPs are calculated as a cubic function of the levels of parameters. If the levels of _hitFreq_ and _maxPay_ are k<sup>th</sup> and l<sup>th</sup> respectively, the RTP is as follows.
 
RTP(k, l) = 1 + c*(k+l-k<sub>mid</sub>-l<sub>mid</sub>)<sup>3</sup>,  
where c = 0.1 / * (max(k+l-k<sub>mid</sub>-l<sub>mid</sub>))<sup>3</sup>
 
Then the resulting RTP would be distributed from 90% to 110%.

* * *

# References

[1] _Global gaming outlook 2011-2015_, PricewaterhouseCoopers, 2011, https://www.pwc.com/gr/en/publications/assets/global-gaming-outlook-2011-2015.pdf, retrieved on July 1st 2017.

[2] _Global online gambling industry size 2009-2020_, Statista, https://www.statista.com/statistics/270728/market-volume-of-online-gaming-worldwide/, retrieved on July 1st 2017.

[3] _Global Online Gambling Market - by Type, Device, Regions - Market Size, Demand Forecasts, Industry Trends and Updates 2014-2020_,
August 2016, Intelliroi, https://www.researchandmarkets.com/research/hdl474/global_online, retrieved on July 1st 2017.

[4] Slot machine, Wikipedia, https://en.wikipedia.org/wiki/Slot_machine#Skill_stops/, retrieved on July 6th 2017.

[5] Dao.Casino Whitepaper, https://github.com/DaoCasino, retrieved on July 1st 2017.

[6] iDice - Ethereum dice beta release, https://iDice.io, retrieved on July 1st 2017.

[7] vDice - The most popular ether betting games in the universe, https://vDice.io, retrieved on July 1st 2017.

[8] Edgeless - Decentralised Edgeless CASINO, https://edgeless.io, retrieved on July 6th 2017.

[9] funfair - The world's fastest Ethereum casino platform, https://funfair.io/, retrieved on July 1st 2017.

[10] RANDAO - A DAO working as RNG of Ethereum, https://github.com/randao/randao, retrieved on July 1st 2017.

[11] Oraclize - blockchain oracle service, enabling data-rich smart contracts, http://www.oraclize.it/, retrieved on July 1st 2017.

[12] random.org - True random number service, https://www.random.org/, retrieved on June 26th 2017.

[13] _State Channels - an explanation_, Jeff Coleman, November 6th 2015, http://www.jeffcoleman.ca/state-channels/, retrieved on June 28th 2017.

[14] _What are State Channels?_, Stephan Tual, January 4th 2017, https://blog.stephantual.com/what-are-state-channels-32a81f7accab, retrieved on June 25th 2017.

[15] Whisper - ethereum/wiki, https://github.com/ethereum/wiki/wiki/Whisper, retrieved on July 1st 2017.

[16] How to whisper - ethereum/go-ethereum/wiki, https://github.com/ethereum/go-ethereum/wiki/How-to-Whisper, retrieved on July 1st 2017.

[16] _Elements Of Slot Design - 2nd Edition_, GameDesignAutomation, 2013, http://slotdesigner.com/wp/wp-content/uploads/Elements-of-Slot-Design-2nd-Edition.pdf, retrieved on June 26th 2017.

[17] Ethereum whitepaper, https://github.com/ethereum/wiki/wiki/White-Paper, retrieved on June 15th 2017.

* * *

# END OF DOCUMENT

* * *
