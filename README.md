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
    db_user = ...
    db_password = ...,
    db_name = ...,
)

@bot.message_handler(commands=['start'])
def send_start_message(message):
    database.register_user(message)
    bot.send_message(message.chat.id, 'Start message...')
```

## Contributors
<div style="display: flex; flex-direction: row; align-items: center;">
<a href="https://github.com/grnbows" style="text-decoration: none; color: unset">
<div style="display: flex; flex-direction: row; align-items: center; margin-right: 40px">
<img src='https://avatars.githubusercontent.com/u/58640700?s=460&u=6c0d0e9a7046256106167426478b1b4232bc118e&v=4' style="width: 100px; height: 100px; border-radius: 50%; margin-right: 20px;"/>
<div> 
<h2 style="margin: 0;">Denis Putnov</h2>
<h4 style="margin: 0;">grnbows</h4>
</div>
</div>
</a>
</div>
