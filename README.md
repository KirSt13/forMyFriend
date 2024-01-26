# Главный текст Markdown

Подтянуть изменения — git pull. Подтягивает в локальный репозиторий последнюю версию проекта. Будьте внимательны, вызов этой команды сотрёт все незафиксированные изменения. Иногда после ввода этой команды появляется конфликт.

Как решать проблемы в Git

Посмотреть статус файлов — git status. Вы увидите, какие файлы изменили, удалили или добавили в проект. При этом статус «Закоммичен» не отобразится.

Добавить файлы в индекс — git add [название файла]. После ввода этой команды вы можете сделать коммит.

Есть похожие команды, например, git add . индексирует сразу все изменённые файлы и папки в директории, где вы находитесь. Обратите внимание, между точкой и словом add нужно ставить пробел. Команда git add :/ добавляет в индекс все файлы независимо от того, в какой директории вы находитесь.

Сделать коммит — git commit -m "Комментарий к коммиту" — фиксирует изменения. До выполнения этой команды локальные изменения никуда не запишутся.

Нужно правильно разбивать изменения и давать полные комментарии к коммитам. Подробнее об этом читайте в статье «Как оформлять коммиты».

Посмотреть историю коммитов — git log. Выводит список всех коммитов. У этой команды есть разные опции, самая используемая из них — --oneline. Она показывает хеш в укороченном формате, ветку, в которой сделан коммит, а также текст коммита. Чтобы использовать эту опцию (как и любую другую), нужно добавить её после команды: git log--oneline.

Запушить изменения — git push. Отправляет все зафиксированные изменения с локального репозитория в удалённый. Это одна из самых важных команд, ведь все вышеописанные действия производятся в локальной копии репозитория.
Когда вы закончите работу, эту копию нужно будет отправить в удалённый репозиторий. Только так другие участники процесса смогут получить актуальную версию.

#Хеш
Хеш - идентификатор коммита в Git.
Хеширование - преобразование набора данных для получения их "отпечатка".
Хеш коммита получается с помощью алгоритма SHA-1.
Хеш состоит из цифр 0-9 и латинских букв A-F.
Свойства хеша: если дважды получить хеш для одного набора данных, результат будет одинаковым.
Если изменить хоть что-то в исходных данных, хеш изменится.
Хеш - основной идентификатор коммита, позволяет узнать автора, дату и содержимое закоммиченных файлов.
Хеши и таблицу хеш → информация о коммите Git сохраняет в служебных файлах в папке .git.