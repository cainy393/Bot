Bot - the intelligent chat bot.
======

Introducing bot version 3! A complete re-write has taken place to make the code a little less messy and more easily understood. Furthermore the bot now takes advantage of my module [DogeChat-Bot](https://github.com/cainy393/DogeChat-Bot) to simplify the process.

This is an open source chat bot written in node.js for the website [DogeChat](http://dogechat.net/) found in the [#bot](http://dogechat.net/join:bot) room. It takes advantage of the socket.io-client npm module to communicate with the site as if it were a client using the chat site.

Installation
------------

To run the bot you must first install node.js and preferably npm for installing its dependencies. From a command window located in the root directory type `npm install` to install the required modules.

Instructions
------------

`<par>` is a required parameter, however you do not need to type the <>

`[par]` is an optional parameter, again you do not need to type the []

### User Balances
To top up your balance simply tip bot an amount.

    /tip bot <amt>

To check your balance use the !bal command as shown below.

    !bal

To cashout your balance it must be over 5 DOGE. You can either cashout your whole balance or a set amount using the command below.

    !cashout [amt]

[amt] is optional, if not specified your whole balance will be tipped to you. If it is specified you will withdraw this amount.

To donate part or all of your balance to the bot to help fund its future development and hosting costs then you can use the donate command shown below.

    !donate [amt]

[amt] is optional, if not specified your whole balance will be donated. If it is specified you will only donate this amount.

### Dice Roll Game

Once you have some DOGE in your balance you can roll the dice to gamble with it. The command is as follows.

    !roll <bet>

Where <bet> is the amount you wish to bet. This will roll 2 dice and display the results. For example if you wanted to bet 20 DOGE you would type:

    !roll 20

The odds for winning are as follows:

  * Double 6 - 4x your bet
  * Double - 2x your bet
  * Single 6 - 1.5x your bet

There is a 4 in 9 chance of winning a prize.

### Doge Ticker

To check the latest price of DogeCoin use the command below. The price of DogeCoin is taken from Cryptsy and the price of Bitcoin for converting into fiat currencies is taken from the [BitcoinAverage Price Index](https://bitcoinaverage.com/).
To simply get the price of DogeCoin in BTC you need not specify any parameters.

    !doge [amount] [currency]
	
Where [amount] is the amount in DogeCoin you wish to convert and [currency] is the fiat currency you wish to convert into (if not specified it will be converted to BTC). The two parameters for this command are both optional.
Supported fiat currency codes are: AUD, BRL, CAD, CHF, CNY, EUR, GBP, HKD, ILS, MXN, NOK, NZD, PLN, RON, RUB, SEK, SGD, TRY, USD and ZAR.

For example if you wanted to check what 1000 DogeCoin was in GBP you could use the command as follows:

    !doge 1000 GBP

This is available in multiple rooms as well as [#bot](http://dogechat.net/join:bot) at the request of certain room owners. If you want this ticker in your room [PM cainy](http://dogechat.net/).

### Currency Conversion

Due to the issues with MtGox this command does not currently work. This will be fixed ASAP.

### Artificial Intelligence

Bot takes advantage of the powerful Wolfram Alpha website to bring you informative artificial intelligence. You can make queries to Wolfram Alpha using the command as shown below:

    !ai <query string>

For example if you wanted to know what the weather was like in New York you could type:

    !ai Whats the weather like in New York?

Or if you prefer:

    !ai weather new york

To learn more about Wolfram Alpha and the ways you can use it please visit [their website](http://www.wolframalpha.com/).

Please do not abuse or excessively use this feature. Without paying for access to Wolfram Alpha bot is limited to 2000 requests per month which isn't many at all (one every 21 minutes). 

### Flirting

You can flirt with other users using the command as shown below:

    !flirt <user>

Where <user> is the user you wish to flirt with.

### Google Search

You can search Google and have the top result returned to you in the chat using the command as shown below:

    !search <query string>

For example if you wanted to search for Bitcoin faucets you could type:

    !search bitcoin faucets

### YouTube Search

You can search YouTube and have the top result returned to you in the chat using the command as shown below:

    !watch <query string>

For example if you wanted to search for funny cat videos you could type:

    !watch funny cats

### GrooveShark Search (Music)

You can search GrooveShark and have the top result returned to you in the chat using the command as shown below:

    !listen <query string>

For example if you wanted to search for Moves Like Jagger you could type:

    !listen moves like jagger

License
-------

MIT License
