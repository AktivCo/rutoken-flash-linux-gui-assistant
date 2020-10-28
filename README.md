# Графическая утилита для разблокировки скрытых защищенных разделов в Рутокен ЭЦП 2.0 Flash в Linux и macOS
Утилита открывает скрытые защищенные разделы на Рутокен ЭЦП 2.0 Flash. Примечания:
1. Изменяются права доступа лишь для локального пользователя l3
2. К открытым разделам можно устанавливать права доступа "Только на чтение" и  "На чтение и запись"
# Загрузка и запуск
```sh
git clone https://github.com/AktivCo/rutoken-flash-linux-gui-assistant --recursive
```
Утилита автоматически проверит наличие необходимых пакетов для работы, и при необходимости попросит их установить. **Установка требует наличия прав супер пользователя**, поэтому утилита запросит пароль администратора во время установки обновлений.

**Для пользователей Astra Linux создан специальный настройщик**, создающий ярлык для запуска приложения без терминала. Просто запустите *token-assistent.installer* и ярлык автоматически появится. 

В остальных операционных системах запуск можно производить двойным щелчком по утилите *token-assistent.run*.

# macOS
Перед началом работы установите последнюю версию [brew](https://brew.sh). Также нужно вручную поставить нуные пакеты для работы:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
brew install python3 openssl libp11 opensc pcsc-lite wget pstree
```
