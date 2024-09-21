# Databricks Genie Bot

## Objective

This project implements an experimental chatbot that interacts with Databricks' Genie API, which is currently in Private Preview and not officially supported (will be updated if it changes). The bot is designed to facilitate conversations with Genie, Databricks' AI assistant, through a chat interface like MS Teams.

## Overview

This experimental code creates a Genie BOT in Databricks using the Genie API. It's important to note that this is not production-ready code and is not associated with or endorsed by any employer. The code is intended to be used as-is for experimental and learning purposes only.

## Key Features

- Integrates with Databricks' Genie API to start conversations and process follow-up messages
- Handles user queries and presents Genie's responses
- Manages conversation state for multiple users
- Formats and displays query results in a readable markdown table
- Handles clarification requests from Genie

## Implementation Details

The bot is built using:
- Python
- Bot Framework SDK
- aiohttp for asynchronous HTTP requests
- Databricks Genie API (Private Preview)

The main components of the system are:
- A `genie_conversation` function that handles the communication with the Genie API
- A `MyBot` class that processes incoming messages and manages user conversations
- An aiohttp web application that serves as the entry point for bot messages

## Disclaimer

This code is experimental and uses a Private Preview API that is not yet supported by Databricks. It should not be used in production environments and is provided strictly for educational and experimental purposes. Use at your own risk.

The code was tested in Azure Bot Framework that facilitates to integrate with any chatbot like MS Teams.

## Setup and Usage

1. Install the required dependencies listed in `requirements.txt`
2. Set up the necessary environment variables (DATABRICKS_SPACE_ID, DATABRICKS_HOST, DATABRICKS_TOKEN, etc.) in the env.example file, change the name to .env
3. Run the `app.py` script to start the bot
4. Call the bot endpoint via Azure Bot Framework or deploy it on a web application to handle the calls.

Please refer to the code comments for more detailed information on each component's functionality.
