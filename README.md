# pytelbot
Pytelbot is the best library for telegram bots making

# pytelbot

The pytelbot library provides a simple toolkit for working with Telegram bots. With this library, you can easily integrate Telegram bot functionalities into your Python applications.

## Installation

You can install the pytelbot library using pip:

bash
pip install pytelbot

## Usage

Here's an example of how you can use the pytelbot library to interact with Telegram's bot API:

python
from pytelbot.telegram_bot_toolkit import TelegramBot

# Initialize the TelegramBot with your bot token
bot = TelegramBot()
bot.init("YOUR_BOT_TOKEN")

# Get updates
updates = bot.get_upd()
print(updates)

# Send a message
bot.send_msg("CHAT_ID", "Hello, this is a test message.")

# Send a photo
bot.send_pht("CHAT_ID", "http://example.com/photo.jpg", "Check out this photo!")

# Send a document
bot.send_doc("CHAT_ID", "http://example.com/docexample.xls", "Check out this document!")

# Send a location
bot.send_loc("CHAT_ID", "latitude", "longitude")

In this example, replace YOUR_BOT_TOKEN with your actual Telegram bot token and CHAT_ID with the appropriate chat ID.

## Methods

### Initialization

python
bot = TelegramBot()
bot.init("YOUR_BOT_TOKEN")

The init method initializes the TelegramBot instance with your Telegram bot token.

### Get Updates

python
updates = bot.get_upd()

The get_upd method retrieves updates from the Telegram bot API.

### Send Message

python
bot.send_msg("CHAT_ID", "Hello, this is a test message.")

The send_msg method sends a message to the specified chat.

### Send Photo

python
bot.send_pht("CHAT_ID", "http://example.com/photo.jpg", "Check out this photo!")

The send_pht method sends a photo to the specified chat.

...

Similarly, you can find descriptions for other methods provided by the pytelbot library.
