# anon.chat

Анонимный чат без регистрации. История исчезает при закрытии вкладки.
Ответы приходят через Telegram-бота.

## Стек
Next.js 15 · Upstash Redis · Telegram Bot API

## Переменные окружения
| Переменная | Где взять |
|---|---|
| TELEGRAM_BOT_TOKEN | @BotFather → /newbot |
| TELEGRAM_CHAT_ID | @userinfobot |
| TELEGRAM_WEBHOOK_SECRET | придумайте (16+ символов) |
| NEXT_PUBLIC_APP_URL | URL приложения |
| UPSTASH_REDIS_REST_URL | upstash.com |
| UPSTASH_REDIS_REST_TOKEN | upstash.com |

## Запуск
```bash
npm install
cp .env.example .env.local
# заполните .env.local
npm run dev
```

## Как пользоваться
1. Напишите сообщение на сайте — оно придёт в Telegram с префиксом `[#sessionId]`.
2. Ответьте **через Reply** на это сообщение.
3. Через 3 секунды ответ появится на сайте.