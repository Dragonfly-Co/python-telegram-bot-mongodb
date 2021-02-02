# Python Telegram Bot MongoDB

Database for python telegram bots based on pyTelegramBotApi with MongoDB. Here it is a base functionality, which is needed for comfortable developming. Library can provide you base interactions with database, users and content.

## Installation

Just download the folder, paste it in you project and import the main class `DataBase`. Create the instance of a class and be happy. 

```
pip[in work]
```

## Usage

```
database = DataBase(
    connection_string = f'mongodb+srv://{config.DB_USER}:{config.DB_PASSWORD}@cluster0.gafny.mongodb.net/{config.DB_NAME}?retryWrites=true&w=majority',
    db_name = config.DB_NAME,
)


@bot.message_handler(commands=['start'])
def send_start_message(message):
    database.register_user(message)
    bot.send_message(message.chat.id, 'Start message...')
```

