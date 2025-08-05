# Telegram Mini App Configuration for MetaQuid

## Bot Setup Instructions

### 1. Create Telegram Bot
1. Message @BotFather on Telegram
2. Use `/newbot` command
3. Choose bot name: `MetaQuid Mining Bot`
4. Choose username: `metaquid_mining_bot` (or similar)
5. Save the bot token

### 2. Configure Mini App
1. Message @BotFather again
2. Use `/mybots` and select your bot
3. Choose "Bot Settings" → "Menu Button"
4. Set Menu Button Text: `🚀 Start Mining`
5. Set Menu Button URL: `https://your-domain.vercel.app`

### 3. Web App Configuration
Send this command to @BotFather:
```
/setmenubutton
@your_bot_username
url - https://your-domain.vercel.app
text - 🚀 Start Mining
```

### 4. Bot Commands Setup
Configure these commands with @BotFather using `/setcommands`:
```
start - 🚀 Start mining and earn money
help - ❓ Get help and instructions
balance - 💰 Check your current balance
withdraw - 💸 Request withdrawal
stats - 📊 View your mining statistics
```

## Webhook Configuration (for production)

### Required Environment Variables
```
TELEGRAM_BOT_TOKEN=your_bot_token_here
WEBHOOK_URL=https://your-domain.vercel.app/api/telegram
```

### Bot Message Handling
The app will send these types of messages to your bot:

1. **User Login**
   ```
   User logged in: John Doe (@johndoe) - ID: 123456789
   ```

2. **Task Completion**
   ```
   Ad task completed. New balance: $2.50
   Daily check-in completed. New balance: $3.00
   Mining boost activated. New balance: $5.00
   ```

3. **Withdrawal Requests**
   ```
   Withdrawal Request:
   Method: bkash
   Account: 01712345678
   Amount: $33.00
   User Balance: $50.00
   ```

## Telegram Mini App Features Enabled

✅ **Automatic Login** - Users are automatically logged in when accessing via Telegram
✅ **User Data Access** - App gets user's name, username, and ID from Telegram
✅ **Native Integration** - App adapts to Telegram's dark theme
✅ **Data Sending** - All user actions are sent back to the bot
✅ **Responsive Design** - Optimized for mobile Telegram interface

## Security Features

- User authentication via Telegram's secure WebApp API
- Encrypted data transmission between app and Telegram
- User ID verification for all transactions
- Automatic session management

## Deployment Notes

When deploying to Vercel:
1. Upload the single `index.html` file
2. Configure custom domain (optional)
3. Set up webhook endpoint for bot notifications
4. Test Mini App functionality through Telegram

The Monetag SDK is properly integrated and will display ads according to your zone configuration (9670918).