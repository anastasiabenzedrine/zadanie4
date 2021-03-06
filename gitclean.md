[< к содержанию](./readme.md)

## **git clean**

Команда **git clean** используется для удаления мусора из рабочей директории. Это могут быть результаты сборки проекта или файлы конфликтов слияний.

Одной из распространённых причин для этого может быть удаление мусора, который был сгенерирован при слиянии или внешними утилитами, или удаление артефактов сборки в процессе её очистки.

Вам нужно быть очень аккуратными с этой командой, так как она предназначена для удаления неотслеживаемых файлов из вашей рабочей директории. Даже если вы передумаете, очень часто нельзя восстановить содержимое таких файлов. Более безопасным вариантом является использование команды **git stash --all** для удаления всего, но с сохранением этого в виде спрятанных изменений.

По умолчанию команда **git clean** будет удалять только неотслеживаемые файлы, которые не добавлены в список игнорируемых. Любой файл, который соответствует шаблону в вашем .gitignore, или другие игнорируемые файлы не будут удалены. 

    git clean 