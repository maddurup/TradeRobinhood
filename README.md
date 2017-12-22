# Robinhood Shell

Robinhood Shell is a command line shell for trading stocks using [Robinhood](https://robinhood.com/).

Commands Supported
------------------ 

* `l` : Lists your current portfolio
* `b <symbol> <quantity> <price>` : Submits a limit order to buy <quantity> stocks of <symbol> at <price>
* `s <symbol> <quantity> <price>` : Submits a limit order to sell <quantity> stocks of <symbol> at <price>
* `q <symbol>` : Get quote (current price) for symbol
* `o` : Lists all open orders
* `c <id>` : Cancel an open order identified by <id> [<id> of a open order can be got from output of `o`]
* `bye` : Exit the shell  

Setup
-----

If you don't have a Robinhood account, sign up for Robinhood. It is a free stock trading platform. Use my [referral link](https://share.robinhood.com/anils31/) to sign up and get one free stock :) 

Download Robinhood Shell by downloading the zip file ([link](https://github.com/maddurup/TradeRobinhood/archive/master.zip)) OR by using git 
```
git clone https://github.com/maddurup/TradeRobinhood.git
```

Install the dependencies
```
sudo pip install -r requirements.txt
```

Create and save your username/password in the config file
```
cp config.py.sample config.py
# Edit config.py - replace username/password with your real username/password
```

You are good to go. Start the shell by
```
chmod +x shell.py
./shell.py
```

Credits
-------
The shell builds on [RobinhoodShell Python API](https://github.com/anilshanbhag/RobinhoodShell.git) by anil

Disclaimer
---------
TradeRobinhood Shell is not associated with the Robinhood app or endorsed by it. 
