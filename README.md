# SCRUM Poker Bot

Simplest Telegram bot for [Scrum Planning Poker](https://en.wikipedia.org/wiki/Planning_poker):
```shell
Scrum-master: Ready? 3... 2... 1... GO!
Alice: 2
Bob: 10
Carol: 5
Scrum-master: ---
ShantiScrumBot: Num votes: 3, average: 6
```

### Install
1. Create new group chat in Telegram
2. Add [@ShantiScrumBot](https://t.me/ShantiScrumBot)
3. Make [@ShantiScrumBot](https://t.me/ShantiScrumBot) group chat admin

### Usage
1. just make votes in chat. A vote is a message containing only a positive integer
2. to get results or to reset current vote send a message with any number of `-` symbols (e.g `-`, `----`, `------`)

Text messages will be ignored. If you want to change your vote, just send a new value to the chat.

```shell
Alice: 222222222222222
Alice: Sorry, cat on keyboard...
Alice: 2
Bob: 4
Scrum-master: ---
ShantiScrumBot: Num votes: 2, average: 3
```

### Run on server (if you want own instance of this bot)
```shell
go get -u github.com/shantchat/tgscrumbot
$HOME/go/bin/tgscrumbot -token '0000000000:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx' -vote-message='Num votes: %d, average: %d' 
```

### Playground 
https://t.me/+oIw9EKVrg8s5MGJi (this is not a bot, this is real demo chat with curious persons)
