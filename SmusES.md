# Instruction #

*Про git, markdown и связанные с ними радости жизни.*

**1. БАЗОВЫЕ КОМАНДЫ**

**init**

инициализация = git следит за тем, что происходит в этой папке, работает с ней. Папка становится **репозиторием**. В папке после инициализации появляется скрытая папка .git . Для "остановки" отслеживания можно удалить данную папку.

**clone**

создание репозитория копированием удаленного репозитория (например с Github).

**status**

информация о работе - репозиторий, что отслеживается, коммиты, история, статус сохранения данных.

**add**

команда подразумевает ввод названия файла через пробел, также можно указать git --all. Команда добавляет в фиксацию, как бы "выделяет" файл для последующей фиксации изменений в системе контроля с помощью commit.

**commit**

непосредственно фиксация изменений в commit, подразумевающий соответствующие комментарии к изменениям git commit -m "..." (message - комментарий к коммиту). **Комментарий обязательно!**

**log**

журнал изменений - какие коммиты есть, информация о них (в том числе уникальные hash по которому их можно найти).

**checkout**

переход к нужной версии файла (по сути к файлу в том состоянии, в котором он был по итогам соответствующего коммита). Перейти между коммитами можно путем ввода первых символов его  hash кода (минимум 4).
НЕ ЗАБЫВАТЬ ВОЗВРАЩАТЬСЯ к актуальной версии файла с помощью checkout master.

**diff**

просмотр разницы между сохраненной версией и тем, что уже зафиксированно в commit.

**branch**

показать имеющиеся в репозитории ветки.
git branch имя_ветки - создание новой ветки.

**2. РАБОТА С УДАЛЕННЫМИ РЕПОЗИТОРИЯМИ**

**clone** 

создание репозитория копированием с github

при этом после данной команды не нужно использовать init

**remote**

"связь" удаленного и локального репозитория (куда будем лить) - указываем основную ветку.

**push**

перемещение в web  сервис

**pull**

вытащить с удаленного репозитория все изменения в локальную.

команда составная, вытаскивает ветку и в т.ч. мержит

**fetch**

вытаскивает всю базу

**pull / push request** 

функции github - запросы на загрузку и выгрузку данных

**3. ФИШИЧКИ**
* Q - выход из меню с информацией (после просмотра status, log);
* подсказки в тексте!;
* в сети есть магическая git book;
* при вводе команд стрелки вверх и вниз - выбор из истории;
* при вводе имени в add внести полное наименование можно с помощью Tab;
* clear - очистить терминал.