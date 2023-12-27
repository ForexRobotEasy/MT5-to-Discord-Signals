# MT5 to Discord Signals

This code allows you to send trading notifications from MetaTrader 5 (MT5) to a Discord channel using the Discord API. It is designed to streamline your trading process by providing real-time updates on your trades directly to your Discord channel.

## Features

- Sends notifications for the following trading events:
  - Order placed
  - Order modified
  - Order executed
  - Order closed
- Customizable notification settings to enable/disable specific notifications
- Easy integration with Discord using the Discord API
- Simple and straightforward code implementation

## Requirements

- MT5 trading platform
- Discord account
- Discord Bot token ([create a bot](https://discord.com/developers/applications))
- Discord channel ID

## Installation

1. Import the necessary libraries by including the `Discord.mqh` file.
2. Set your Discord Bot token and channel ID in the `DISCORD_TOKEN` and `DISCORD_CHANNEL_ID` constants, respectively.
3. Customize the notification settings according to your preferences by modifying the `notifyOrdersPlaced`, `notifyOrdersModified`, `notifyOrdersExecuted`, and `notifyOrdersClosed` boolean flags.
4. Initialize the Discord client in the `OnInit()` function.
5. Subscribe to trading events in the `OnInit()` function.
6. Implement the `OnTrade()` function to handle trading events.
7. Use the `SendNotification()` function to send notifications to your Discord channel.
8. Disconnect from Discord in the `OnDeinit()` function.
9. Register the trading event function in the `start()` function.

## Usage

1. Compile and run the code in your MT5 trading platform.
2. Make sure the Expert Advisor is enabled and running.
3. Anytime a trading event occurs (order placed, modified, executed, or closed), a notification will be sent to your Discord channel.

## Disclaimer

Please note that this code is a sample provided by Forex Robot Easy Team and is not the official product. We only provide this code as an example of how the product works. For detailed reviews and trading results of the official product, please visit [here](https://forexroboteasy.com/forex-robot-review/mt5-to-discord-signals-streamline-trading-with-review/). To find the official developer of this product, please refer to the MQL5 platform.

For any issues or questions regarding the code, please contact the official developer of the product.

For more information and updates, please visit [Forex Robot Easy](https://www.forexroboteasy.com).

**Backlink**: For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/mt5-to-discord-signals-streamline-trading-with-review/).
