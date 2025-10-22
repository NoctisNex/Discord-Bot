# 🤖 Discord Bot

> My first big Python project - A feature-rich Discord bot built with discord.py

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![Discord.py](https://img.shields.io/badge/Discord.py-2.0+-green.svg)](https://github.com/Rapptz/discord.py)
[![Status](https://img.shields.io/badge/Status-Abandoned-red.svg)](README.md)

A versatile Discord bot that combines moderation tools, fun commands, and music capabilities. This project represents my journey into Python development and Discord bot creation.

## ✨ Features

### 🎵 Music System
- **Lavalink Integration**: High-quality music streaming
- **Queue Management**: Add, skip, and manage music queues
- **Multiple Sources**: Support for various music platforms

### 🛡️ Moderation Tools
- **Message Purging**: Bulk delete messages with `+purge`
- **Role-based Access**: Commands restricted to specific roles
- **Safe Shutdown**: Graceful bot shutdown with `+close`

### 🎮 Fun Commands
- **Personalized Greetings**: Special hello messages for specific users
- **Interactive Commands**: Punch, info, and custom responses
- **Channel-specific Features**: Commands that work in designated channels

### 📊 Logging & Monitoring
- **Comprehensive Logging**: All bot activities logged to `discord.log`
- **Debug Support**: Detailed logging for troubleshooting
- **Message Tracking**: Monitor user interactions and commands

## 🚀 Quick Start

### Prerequisites
- Python 3.10 or higher
- Discord Bot Token
- Lavalink server (for music features)

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd discord-bot
   ```

2. **Install dependencies**
   ```bash
   pip install discord.py
   pip install discord.py[voice]  # For music features
   ```

3. **Configure the bot**
   - Replace the `TOKEN` in both `main.py` and `command.py` with your Discord bot token
   - Update the Lavalink server credentials in `command.py`
   - Modify role IDs and channel IDs as needed

4. **Run the bot**
   ```bash
   python main.py
   ```

## 📋 Commands

| Command | Description | Permission |
|---------|-------------|------------|
| `+hello` | Personalized greeting message | Everyone |
| `+punch <user>` | Punch another user (channel-specific) | Everyone |
| `+info` | Display server, user, and message info | Everyone |
| `+purge <number>` | Delete specified number of messages | Everyone |
| `+close` | Shutdown the bot | Developer role only |
| `+krapfen` | Berliner vs Krapfen debate | Everyone |

## 🏗️ Project Structure

```
discord-bot/
├── main.py              # Main bot file with logging setup
├── command.py           # Bot commands and music integration
├── discord.log          # Bot activity logs
├── __pycache__/         # Python cache files
└── README.md           # This file
```

## 🔧 Configuration

### Bot Token Setup
1. Go to [Discord Developer Portal](https://discord.com/developers/applications)
2. Create a new application
3. Navigate to the "Bot" section
4. Copy the token and replace it in the code

### Lavalink Setup
For music features, you'll need a Lavalink server:
```python
bot.lavalink_nodes = [
    {"host": "your-lavalink-host", "port": 2124, "password": "your-password"},
]
```

### Role Configuration
Update role IDs in the code to match your Discord server:
```python
@commands.has_any_role("Developer", 748618875180154980)
```

## 🎯 Learning Outcomes

This project helped me understand:
- **Object-Oriented Programming**: Working with classes and methods
- **Async/Await**: Asynchronous programming with Python
- **API Integration**: Working with Discord's API and external services
- **Error Handling**: Implementing proper logging and error management
- **Code Organization**: Structuring code across multiple files
- **Version Control**: Managing code with Git

## 🛠️ Technologies Used

- **Python 3.10+**: Core programming language
- **discord.py**: Discord API wrapper
- **Lavalink**: Music streaming service
- **Logging**: Built-in Python logging module

## 📝 Notes

- This was my first major Python project
- The bot includes both basic and advanced Discord features
- Music functionality requires a separate Lavalink server
- Some commands are specific to certain Discord servers/channels

## ⚠️ Project Status

**This project is abandoned and no longer maintained.** It was created as a learning exercise and is preserved for historical purposes.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Built with ❤️ and lots of Python - My first big Python project*