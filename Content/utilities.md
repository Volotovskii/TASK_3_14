## Утилиты

* `git status` - Показывает состояние текущего рабочего каталога и области подготовки.
* `git log` - Показывает историю коммитов.
* `git diff` - Показывает разницу между двумя коммитами или между коммитом и рабочим каталогом.

## git status

### Описание
Команда `git status` используется для отображения состояния текущей рабочей области и индекса. Она предоставляет информацию о следующих элементах:

* Измененные, но не добавленные в индекс файлы
* Добавленные в индекс, но не зафиксированные файлы
* Удаленные файлы
* Неотслеживаемые файлы (не находящиеся под управлением Git)

### Применение
* **Проверка состояния изменений:** Определите, какие файлы изменены, добавлены или удалены в вашей рабочей области или индексе.
* **Обзор незафиксированных изменений:** Проверьте, какие изменения были добавлены в индекс, но еще не зафиксированы.
* **Поиск неотслеживаемых файлов:** Найдите файлы, которые не отслеживаются Git, но присутствуют в вашей рабочей области.

**Пример:**

```
git status
```

Вывод команды будет выглядеть примерно так:

```
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

  task_3_14.txt

no changes added to commit (use "git add" and/or "git commit -a")
```

## git log

### Описание
Команда `git log` используется для отображения истории коммитов в репозитории. Она предоставляет информацию о каждом коммите, включая хеш коммита, автора, дату коммита и сообщение о коммите.

### Применение
* **Просмотр истории изменений:** Осмотрите историю коммитов проекта, чтобы увидеть, кто внес какие изменения и когда.
* **Отслеживание изменений:** Проследите за развитием проекта, просматривая коммиты по порядку.
* **Поиск конкретных коммитов:** Найдите коммиты с помощью опций фильтрации, таких как поиск по автору, диапазону дат или фразе в сообщении коммита.

**Пример:**

```
git log
```

Вывод команды будет выглядеть примерно так:

```
commit 1234567890abcdef
Author: John Doe <task@example.ru>
Date:   Mon Jan 1 00:00:00 2023 -0800

    Fix: Исправлена ошибка в функции X

commit 0987654321fedcba
Author: Jane Smith <task_3_14h@example.ru>
Date:   Sun Dec 31 23:59:59 2022 -0800

    feat: Добавлена новая функция Y
```

## git diff

### Описание
Команда `git diff` используется для отображения различий между двумя коммитами, ветками или файлами. Она показывает измененные строки, а также любые добавленные или удаленные строки.

### Применение
* **Просмотр изменений между коммитами:** Сравните два коммита, чтобы увидеть, какие изменения были внесены.
* **Просмотр изменений между ветками:** Сравните две ветки, чтобы определить различия между ними.
* **Просмотр изменений в файле:** Сравните две версии файла, чтобы увидеть, что было изменено.

**Пример:**

```
git diff HEAD~2
```

Вывод команды будет выглядеть примерно так:

```
diff --git a/task_3_14.txt b/task_3_14.txt
index 1234567890abcdef..0987654321fedcba 100644
--- a/task_3_14.txt
+++ b/task_3_14.txt
@@ -1,3 +1,4 @@
 Это мой файл.
+Добавлена новая строка.
 Я изменил эту строку.
 Удалил эту строку.
```

## Сценарии применения

### Использование `git status`, `git log` и `git diff` вместе
Эти три команды часто используются вместе для управления изменениями в репозитории:

* **Проверка состояния и истории:** Используйте `git status` для проверки состояния вашей рабочей области, а затем `git log` для просмотра истории коммитов.
* **Сравнение изменений:** Используйте `git diff` для сравнения двух коммитов или веток, чтобы увидеть, какие изменения были внесены.
* **Исправление ошибок:** Используйте `git log` для поиска коммита, вызвавшего ошибку, а затем `git diff` для просмотра различий между этим коммитом и предыдущим.

**Важно:** Команда `git diff` не изменяет ваш репозиторий. Она просто отображает различия между двумя состояниями.

### <a href="/readme.md" style="color: red; text-decoration: underline;text-decoration-style: dotted;">***~~Оглавление~~***</a>