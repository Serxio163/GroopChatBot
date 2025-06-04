# GroopChatBot
Бот участник групповых чатов
Инструкция по запуску Telegram бота для групповых чатов
📋 Предварительные требования
Аккаунт Telegram

Созданный Telegram бот через @BotFather

API ключ от Groq

Google Colab или локальный Python 3.11+ окружение
Замените ВАШ_TELEGRAM_BOT_TOKEN и ВАШ_GROQ_API_KEY на свои реальные ключи
Скопируйте код или скачайте файл
Запустите ячейку (Ctrl+Enter или кнопка Play)
⚙️ Настройка бота
Получите токен бота у @BotFather

Добавьте бота в групповой чат

Сделайте бота администратором чата (для правильной работы)

🛠 Управление ботом
Для остановки бота в Colab нажмите Stop в панели управления

Для остановки локального бота нажмите Ctrl+C в терминале

📊 Проверка работы
Отправьте сообщение в групповой чат

Проверьте логи в Colab или терминале

Для просмотра сохраненных данных выполните:
import sqlite3
conn = sqlite3.connect('chat_bot.db')
cursor = conn.cursor()
cursor.execute("SELECT * FROM chat_interactions")
print(cursor.fetchall())
conn.close()
