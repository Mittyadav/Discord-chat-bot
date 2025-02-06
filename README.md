## DISCORD AUTO CHAT BOT

Auto send chat on discord specific channel, good for push rank level on MEE bot and another level basead bot.

## SETUP & CONFIGURE BOT

1. Clone Project Repository
   ```bash
   git clone https://github.com/Rambeboy/discord-chat-bot && cd discord-chat-bot
   ```
2. Install Dependencies
   ```bash
   npm install
   ```
3. Configure Enviroment Variable
   ```bash
   nano .env
   ```
   Environment Example
   ```bash
   DISCORD_EMAIL=YOUR@EMAIL
   DISCORD_PASSWORD=YOURPASSWORD
   USE_QR=1 for ON 0 for OFF
   TARGET_CHAT_CHANNEL=https://discord.com/channels/123123/123123123
   DELAY_EACH_CHAT_IN_SECONDS=70
   HEADLESS=1 for ON 0 for OFF
   BROWSEREXECUTABLEPATH=/path/to/chrome.exe or chrome(bin) you can leave it blank to set it to default path
   ```
5. Run the Bot
   ```bash
   npm run start
   ```

## NOTE

if you want to see browser pop up , edit HEADLESS on .env to false
Change the `/src/utils/messages.js` with your word list

## ADDITIONAL SETUP ON UBUNTU
```bash
sudo apt-get update
sudo apt-get install chromium-browser
sudo mkdir -p /opt/google/chrome
sudo ln -sf $(which chromium-browser) /opt/google/chrome/chrome
```

## LICENSE

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.