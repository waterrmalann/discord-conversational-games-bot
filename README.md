# 🤖 Conversational Game Bot (for Discord: Chat App)

A simple, conversational games bot for Discord to help keep chats active and fun. Responses are stored locally in `.txt` files. The default database is SFW, though it's easy to add or remove responses by editing the text files found in the data folder.

Conversational games the bot has at the moment. You can get a list of commands by typing `/help`.
- **Truth Or Dare**
- **Never Have I Ever**
- **[Would You Rather](http://either.io/)**
- **This Or That**
- **[Will You Press The Button](https://willyoupressthebutton.com/)**

## 🚀 Getting Started

### Inviting

An instance of the bot is hosted publically which you can invite using [this link](https://discord.com/api/oauth2/authorize?client_id=793051926953984000&permissions=280640&scope=bot). However, if you plan on self-hosting the bot, follow the steps down below.

### Prerequisites

- [Python](https://www.python.org/) 3.8 or above.
- [discord.py](https://pypi.org/project/discord.py/) (API Wrapper)

### Installing

1. Clone the repository. (I recommend making a virtual environment)
```
git clone https://github.com/waterrmalannk/discord-conversational-games-bot.git
```
2. Install the requirements.txt
```
python -m pip install -r requirements.txt
```
3. Create a bot application and grab a token from [here](https://discord.com/developers/applications/me).
4. Open `config.json` and put the bot token in `BOT_TOKEN`. Also edit any other settings you want to edit like the prefix.
5. Run the project
```
python cgb.py
```

### Adding new responses or editing them.

Responses are located at the data folder in text files where they're separated using newlines. Currently, local response databases exist only for Truth or Dare, Never Have I Ever, and This or That. Would You Rather and Press The Button works by requesting their websites to fetch questions. I do plan on also making a local database for both of these games just in case the request approach fails or stops working in the future.

## 🤝 Contributing

Contributions are accepted and there really isn't any strict rules. Feel free to open a pull request to fix any issues or to make improvements you think that should be made. You can also add new games or new responses to the current local database. Any contribution will be accepted as long as it doesn't stray too much from the objective of the bot. If you're in doubt about whether the PR would be accepted or not, you can always open an issue to get my opinion on it.

### To-Do

You can also help me with the current to-do list I have in mind (in no particular order).
- Avoid repetition of the same response for the same person.
- Larger database of questions.
- Backup local database of questions for press the button and would you rather.
- Ability to add custom responses per-guild. (maybe)
- Ability to request responses to be added to the main database (through a command).
- NSFW Database of questions that show up only in nsfw ticked channels.

License
----

AGPLv3, see [LICENSE](LICENSE)