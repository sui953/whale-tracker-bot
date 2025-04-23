# whale-tracker-botimport telebot

API_TOKEN = 'YOUR_BOT_TOKEN'  # Bu yerga bot tokeningizni yozing
bot = telebot.TeleBot(API_TOKEN)

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "Salom! Bu Whale Tracker bot.")

bot.polling()