# khooylowbot
The Khooylowbot is a Telegram bot written in Python that reduplicates the last word of a message in Russian using a specific rule set or randomly selected phrases. The script uses the Telegram Bot API and the python-telegram-bot library.
    
    Setup:
    Before using the Khooylowbot script, you need to create a Telegram Bot and get its API token. To do this, follow the instructions provided in the Telegram Bot API documentation.

After getting the API token, insert it into the BOT_TOKEN variable in the script.

    Functionality:
    The Khooylowbot script performs the following actions:

    Reduplicates the last word of a message in Russian using a specific set of rules or random phrases
    Removes punctuation from the last word before reduplicating it
    Ignores messages that do not contain Cyrillic characters
    Logs errors that occur during the bot's operation
    Handles messages from both group chats and private conversations

    Code Breakdown:
    The Khooylowbot script consists of the following parts:

    Importing libraries: The script imports the necessary libraries such as os, logging, re, random, and the python-telegram-bot library.
    Defining the BOT_TOKEN variable: This variable contains the Telegram Bot API token that the script uses to communicate with the Telegram Bot API.
    Defining the lexical_reduplication function: This function takes a word as input, applies a set of rules to reduplicate it, and returns the reduplicated word.
    Defining the contains_cyrillic function: This function takes a string as input and returns a Boolean value indicating whether the string contains Cyrillic characters.
    Defining the remove_punctuation function: This function takes a string as input and removes any punctuation characters from it.
    Defining the error_handler function: This function takes an Update object and a CallbackContext object as input, logs any errors that occur during the bot's operation, and provides a generic error message to the user.
    Defining the reduplicate function: This function takes an Update object and a CallbackContext object as input, extracts the last word from the message, applies the appropriate reduplication rule to it, and sends the reduplicated word as a reply to the user.
    Defining the main function: This function sets up the logging system, creates an Updater object with the BOT_TOKEN, adds the error_handler and reduplicate functions as handlers, and starts polling the Telegram Bot API for new messages.
    Starting the script: The name == "main" condition ensures that the main function is only called if the script is run directly and not imported as a module.

    Usage:
    To use the Khooylowbot script, follow these steps:

    Insert the Telegram Bot API token into the BOT_TOKEN variable.
    Run the script.
    Add the bot to a group chat or start a private conversation with it.
    Type a message that contains a word in Russian.
    The bot will reduplicate the last word of the message and send the reduplicated word as a reply.

    Conclusion:
    The Khooylowbot script provides a simple example of how to create a Telegram bot that reduplicates words using specific rules or random phrases. The script can be modified to add more reduplication rules or to perform other text processing tasks.
