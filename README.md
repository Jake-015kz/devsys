# System Helper for EndeavourOS 🚀
---


**System Helper** — мощный и стильный Bash-скрипт для управления системой **EndeavourOS** (и других Arch-based дистрибутивов).  
С интерактивным интерфейсом на базе `fzf`, прогресс-барами 🌑🌒🌓, спиннерами и KDE-уведомлениями, он делает администрирование системы удобным и приятным.  

---

## ✨ Возможности

- 🆙 **Быстрое обновление:** через `pacman` или `paru`, с автоматической очисткой кэша.
- 🗑 **Удаление программ:** выбор пользовательских, системных или сиротских пакетов через `fzf`, с описаниями.
- 🧹 **Очистка системы:** удаление кэша, логов и ненужных зависимостей.
- 📊 **Мониторинг памяти:** RAM, ZRAM и Swap с прогресс-барами.
- 🛠 **Управление сервисами:** через `systemctl` с выбором в `fzf`.
- 📜 **Просмотр логов:** через `lnav`.
- 💾 **Анализ диска:** отображение самых крупных директорий.
- ⚡ **Питание:** выключение, перезагрузка, гибернация, сон и таймер выключения.

---

## 📦 Установка

```bash
git clone https://github.com/твой_юзернейм/system_helper.git
cd system_helper
chmod +x system_helper.sh
```

## Установка зависимостей:
```bash
sudo pacman -S fzf libnotify figlet
# Опционально:
sudo pacman -S paru
```

* fzf — интерактивные меню

* libnotify — уведомления KDE (опционально)

* figlet — ASCII-арт (опционально)

* paru — для работы с AUR (опционально)

## 🖥 Использование
```bash
./system_helper.sh
```

### Управление через меню fzf:

    Стрелки ↑↓ — навигация

    Пробел — множественный выбор

    Enter — подтверждение

### Примеры:

    ✅ Обновление: "Обновить через pacman 📦" или "через paru 📥"

    🗑 Удаление программ: выберите категорию и нужные пакеты

    🧹 Очистка: удаление кэша, логов и ненужных зависимостей

    📊 Анализ памяти: отображение RAM, ZRAM, Swap

    🛠 Сервисы: запуск, отключение, перезапуск и просмотр статуса

    ⚡ Питание: выбор действия, установка таймера

---


## 📺 Пример вывода
```textplain
╔════════════════════════════════════════╗
║          ОБНОВЛЕНИЕ PACMAN 📦          ║
╚════════════════════════════════════════╝
Введите пароль для sudo:
Очистка кэша pacman... ✅
Обновление системы... 🌑🌒🌓
[██████████████████████████████] 100%
Обновление завершено. Обновлено пакетов: 6 ✅
```

---


## ⚙️ Требования

    ОС: EndeavourOS или любой Arch-based дистрибутив

    Права: Некоторые функции требуют sudo

    Зависимости: pacman, fzf, libnotify (опц.), figlet (опц.), paru (для AUR)


## 📜 Лицензия

Этот проект распространяется под лицензией MIT — см. LICENSE для подробностей.

```tetx
MIT License

Copyright (c) 2025 [твой_юзернейм]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 👨‍💻 Автор

zhegan kz
GitHub: jake_015kz

---

### 🤝 Контрибьютинг

Предложения, улучшения и PR приветствуются!
Создавайте issues или pull requests, если хотите внести вклад в проект.

---

#### Сделано с ❤️ для сообщества EndeavourOS.
