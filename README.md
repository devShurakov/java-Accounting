# Автоматизация бухгалтерии. Java-accounting.
#### Учебный проект. Обновленная версия с javaDoc

Описание:

Консольное приложение, обработки отчетов.

![Java](https://img.shields.io/badge/-Java-green) ![Git](https://badgen.net/badge/icon/github?icon=github&label)


### Функциональность:
* консольный интерфейс для управления программой.
* считывание месячных и годовых отчётов из файлов и приведение их в объекты приложения.
* сверка данных по месячным и годовым отчётам.
* вывод информацию о месячных и годовом отчёте.

### Дополнительная информация:

* Месячный отчёт, содержащий данные о доходах и расходах в рамках одного календарного месяца. В программе они представляются классом MonthlyReport.
* Годовой отчёт, содержащий ровно по 2 записи на каждый из 12 месяцев — общий доход и расход за этот месяц. Представлен классом YearlyReport.
* Каждый файл в формате CSV состоит из набора строк. В самой первой строке идут заголовки полей. Далее каждая строка состоит из значений, разделённых символов-разделителем — запятой.

### Используемые паттерны:
Singleton(Одиночка)- это шаблон проектирования, который предоставляет нам две вещи:
Гарантия, что у нужного класса будет всего один экземпляр.
Предоставляет глобальную точку доступа к экземпляру данного класса

В коде представлена реализация Simple Solution(не ленивая инициализация).

### Как посмотреть документацию?

* Cкачиваем проект
* Переходим в папку exportToHTML 
* Запускаем файл index

![This is an image](https://github.com/devShurakov/java-Accounting/blob/main/pic.png)


### Обновления:

* Добавлен Pom.xml
* Добавлен плагин maven-doc и описание основных классов и методов. Для знакомства с созданиям документации.
* Добавлен класс Engine отвечающий за основную логику обработки отчетов.
* Добавлен класс FileReader отвечающий за основную логику cчитывания данных из файла.
* Внедрен паттерн проектирования singleton в класс Engine.
