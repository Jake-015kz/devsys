# 🛠️ devsys — мощный CLI-инструмент для обслуживания системы (Arch/EndeavourOS)

`devsys` — это продвинутый системный помощник для Arch-совместимых дистрибутивов.  
Он помогает:

- 🧹 очищать систему (логи, кэш, сироты)
- 🚀 обновлять пакеты
- 🔍 смотреть статистику памяти и zram
- 🧠 управлять сервисами
- 📦 находить и удалять мусорные зависимости
- 🧪 проводить тестирование и диагностику
- 🧩 поддерживает автообновление
- 🎛️ имеет красивое ASCII-меню с выбором действий через `fzf`

---

## 📸 Скриншот

<!-- Загрузить можно на imgur или githubusercontent -->
![devsys-preview](https://github.com/user-attachments/assets/9ec7b2cb-7314-45d8-a373-0daf26011b18)

---

## ⚙️ Установка

```bash
git clone git@github.com:Jake-015kz/devsys.git ~/.local/share/devsys
chmod +x ~/.local/share/devsys/devsys
ln -s ~/.local/share/devsys/devsys ~/.local/bin/devsys
```

Или добавьте в `.zshrc`:

```sh
alias devsys="~/.local/share/devsys/devsys"
```

---

## 📋 Зависимости

Чтобы `devsys` работал на 100%, убедитесь, что установлены:

```bash
sudo pacman -S --needed \
  base-devel git zram-generator \
  fzf lm_sensors pacman-contrib \
  reflector lsof ncdu
```

Для AUR-поддержки:

```bash
sudo pacman -S paru
```

---

## 🔧 Возможности

| №  | Действие                           | Что делает                                                   |
|----|------------------------------------|--------------------------------------------------------------|
| 1  | 📦 Обновление системы              | `paru -Syu`, обновление зеркал, ключей                      |
| 2  | 🧹 Очистка мусора                  | Логи, кэш, сироты, orphan-пакеты, временные файлы            |
| 3  | 🧠 Память и zram                   | `free -h`, `zramctl`, показ использования ОЗУ/подкачки       |
| 4  | 🚨 Логи и ошибки                   | `journalctl -p 3 -xb` и `dmesg`                              |
| 5  | 🧊 Список сервисов                 | `systemctl list-units --type=service`                        |
| 6  | ⏳ Время загрузки                  | `systemd-analyze` и `systemd-analyze blame`                  |
| 7  | 🔥 Самые тяжёлые процессы          | `ps aux --sort=-%mem | head -n 20`                          |
| 8  | 📂 Самые тяжёлые директории        | `ncdu /` или `du -shx /*`                                   |
| 9  | 🔌 Меню: Включить/отключить сервис | Через `fzf` выбери systemd-сервис и включи/отключи           |
| 10 | 💀 Удалить ненужные зависимости    | `pacman -Rns $(pacman -Qdtq)`                               |
| 11 | ❌ Удалить AUR-пакеты вручную      | Через `paru -Rns`                                           |
| 12 | 🔚 Выход                           | Завершение программы                                         |

---

## 📊 Пример отчёта

```bash
✔ Освобождено: 204MB (логи, кэш, сироты)
✔ Orphan-пакетов удалено: 7
✔ Обновлено: 114 пакетов
✔ ZRAM: Используется 623MB из 2GB
```

---


## 🙌 Автор

Разработано Евгением (@Jake-015kz)  
Сконфигурировано под **Plasma + Zsh + Tiling workflow**

---

## ⭐ Если понравился проект

Поставь ⭐ на GitHub и поделись скриптом с друзьями!

```bash
git clone https://github.com/Jake-015kz/devsys.git
```

---

