<h1 align="center">Airtable to Telegram Notifier </h1>

## Project Overview 

Airtable to Telegram Notifier (ATT Notifier) is a seamless integration tool designed to push updates from Airtable to a Telegram channel. Whenever there's a change of status in your Airtable entry, ATT Notifier makes sure your Telegram audience is the first to know! 

## 2\. Features 

- **Real-time Notifications**: Get immediate updates on Telegram for any change in status in your Airtable entry.
- **Image Support**: Push images along with your notifications.
- **Formatted Data Push**: Send your Airtable data in a clean and formatted manner.
- **Scalable & Modular**: Designed with scalability in mind, ensuring easy additions and modifications.

#### Future Enhancements (To-Do) 

- Integrate with multiple Airtable bases.
- Allow custom formatting for Telegram messages.
- Support for other messaging platforms like Slack or WhatsApp.
- Advanced error handling and retry mechanisms.


## Requirements 

- Python 3.8+
- `requests` library
- Airtable API Key
- Telegram Bot Token and Chat ID


## Usage Examples 
```from modules.airtable.airtable_api import fetch_changed_entries, prepare_data_for_telegram
from modules.telegram.telegram_api import send_message_to_telegram

records = fetch_changed_entries()
if records:
    text = prepare_data_for_telegram(records)
    send_message_to_telegram(text)
```

## Setup and Installation Instructions 

1. Clone the repository: `git clone https://github.com/YourUsername/ATT-Notifier.git`
2. Navigate to the project directory: `cd ATT-Notifier`
3. Install the required Python packages: `pip install -r requirements.txt`
4. Update the placeholders in the code with your Airtable API key, Base ID, Telegram Bot Token, and Chat ID.
5. Run `main.py`: `python main.py`


## Troubleshooting Tips 

- Ensure you've set the correct API keys and tokens.
- Check your internet connection.
- Ensure that the Telegram bot has the necessary permissions to post messages.
- Check the Airtable API limits and ensure you're not exceeding them.


## Contribution Guidelines

1. Fork the repository.
2. Create a new branch for your features or bug fixes.
3. Commit your changes with meaningful commit messages.
4. Open a pull request, and describe the changes you've made.
5. Once reviewed, your changes will be merged!
