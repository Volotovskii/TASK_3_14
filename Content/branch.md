## Команда git branch

* `git branch <имя_ветки>` - Создает новую ветку с указанным именем.
* `git checkout <имя_ветки>` - Переключается на указанную ветку.
* `git merge <имя_ветки>` - Сливает изменения из указанной ветки в текущую ветку.

Описание:

Команда git branch используется для создания, перечисления, переименования и удаления ветвей в локальном репозитории Git. Ветви - это параллельные ветки истории коммитов, которые позволяют разработчикам работать над разными функциями или исправлениями независимо друг от друга.

Синтаксис:
```
git branch [опции] [имя ветки]
```


Сценарии применения:

* Создание новых веток: Создание новых веток для работы над новыми функциями или исправлениями.
* Перечисление существующих веток: Перечисление всех существующих веток в локальном репозитории.
* Переименование веток: Изменение имени существующей ветки.
* Удаление веток: Удаление веток, которые больше не нужны или были объединены в основную ветку.
* Просмотр текущей ветки: Отображение текущей ветки, на которой находится рабочий каталог.

## Команда git checkout

Описание:

Команда git checkout переключает рабочий каталог на указанную ветку или создаёт новую ветку и переключается на неё.

Синтаксис:
```
git checkout [опции] [имя ветки или путь]
```


Сценарии применения:

* Переключение между ветками: Переключение рабочего каталога на другую ветку для продолжения работы над ней.
* Создание и переход на новую ветку: Создание новой ветки и немедленное переключение на неё.
* Восстановление удалённых изменений: Переключение на удалённую ветку и извлечение её изменений в локальный рабочий каталог.
* Извлечение конкретного коммита: Переключение на конкретный коммит и создание временной рабочей ветки для его проверки.

## Команда git merge

Описание:

Команда git merge объединяет изменения из одной или нескольких веток в текущую ветку.

Синтаксис:
```
git merge [опции] [ветка или коммит]
```



Сценарии применения:

* Объединение веток: Объединение изменений из другой ветки в текущую ветку.
* Разрешение конфликтов слияния: Разрешение любых конфликтов, которые возникают при слиянии двух веток.
* Обратная интеграция исправлений: Перенос исправлений из одной ветки в другую.
* Создание веток слияния: Создание временной ветки для разрешения конфликтов слияния перед объединением изменений в основную ветку.

### <a href="/readme.md" style="color: red; text-decoration: underline;text-decoration-style: dotted;">***~~Оглавление~~***</a>

