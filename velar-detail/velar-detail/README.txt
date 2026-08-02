VELAR DETAIL — Landing Page
===========================

Структура:
  index.html      — главная страница
  css/style.css   — все стили
  js/app.js       — скрипты

Запуск:
  1. Распакуйте ZIP.
  2. Откройте index.html в браузере.
  3. Для разработки используйте VS Code + Live Server.

Публикация на GitHub Pages:
  1. Создайте репозиторий.
  2. Загрузите файлы.
  3. Settings → Pages → main / root.

Настройка формы:
  В js/app.js замените setTimeout в send() на:

  // Telegram
  fetch('https://api.telegram.org/bot<TOKEN>/sendMessage',{
    method:'POST',
    headers:{'Content-Type':'application/json'},
    body:JSON.stringify({chat_id:'<ID>',text:`Заявка: ${name} ${phone}`})
  })

  // Google Sheets (Apps Script)
  fetch('https://script.google.com/macros/s/<ID>/exec',{method:'POST',body:new FormData(form)})

Контакты:
  Замените +7 (999) 123-45-67 и wa.me/79991234567 на свои.
