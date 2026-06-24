import schedule
import time
import random
from telegram import Bot

TOKEN = "8721671132:AAG_yHQ2v-Kmfp0I4D79nN8cPzMB86d_emU"
GROUP_ID = -1002514952451

messages = [
    "🔥 @ARSHIA_TO عملیات خشم ارمنی دور جدید! آماده باش",
    "💀 @ARSHIA_TO عرشیا، خوابیدی؟ دوباره وقت تنبیه‌ست",
    "⚜️ @ARSHIA_TO سید پیشوا هنوز رحم کرده، زود باش جواب بده",
    "🎯 @ARSHIA_TO موشک جدید رسید عرشیا، فرار کن",
    "🤡 @ARSHIA_TO عرشیا جان، اینقدر ژ ژ نکن، یه حرف حسابی بزن",
    "💎 @ARSHIA_TO اتحاد خاورمیانه منتظر جوابت نیست، حرکتی کن",
    "👑 @ARSHIA_TO سید پیشوا فرمان داد، تو باید جواب بدی",
    "💢 @ARSHIA_TO بی‌تمدن، کی فکر کردی می‌تونی سکوت کنی؟",
    "🔪 @ARSHIA_TO تیغ برای گردنت تیزه"
]

def send_message():
    bot = Bot(token=TOKEN)
    message = random.choice(messages)
    try:
        bot.send_message(chat_id=GROUP_ID, text=message)
        print(f"✅ Message sent: {message}")
    except Exception as e:
        print(f"❌ Error: {e}")

if name == "main":
    send_message()
