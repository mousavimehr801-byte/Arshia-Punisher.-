
import random
from telegram import Bot

TOKEN = "8721671132:AAG_yHQ2v-Kmfp0I4D79nN8cPzMB86d_emU"
GROUP_ID = -1002514952451

msgs = [
    "🔥 @ARSHIA_TO عملیات خشم ارمنی",
    "💀 @ARSHIA_TO خوابیدی عرشیا؟",
    "⚜️ @ARSHIA_TO سید پیشوا صدا میزنه",
    "🎯 @ARSHIA_TO موشک جدید رسید",
    "🤡 @ARSHIA_TO یه حرف حسابی بزن",
    "💎 @ARSHIA_TO اتحاد منتظرته",
    "👑 @ARSHIA_TO سید پیشوا فرمان داد",
    "💢 @ARSHIA_TO بی‌تمدن سکوت نکن",
    "🔪 @ARSHIA_TO تیغ برای گردنت تیزه"
]

bot = Bot(token=TOKEN)
try:
    bot.send_message(chat_id=GROUP_ID, text=random.choice(msgs))
    print("✅ فرستاده شد")
except Exception as e:
    print("❌ خطا:", e)
