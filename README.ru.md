# Java Pro (Tel-Ran, 2022)

[English](README.md) | [Русский](README.ru.md)

Примеры и домашние задания из профессионального курса Java в Tel-Ran. В репозитории есть собственные коллекции, объектные модели, API-клиенты, многопоточный код, работа с базой данных и модульные тесты.

## Что посмотреть

| Тема | Примеры |
| --- | --- |
| Классы, наследование, перечисления и интерфейсы | [lesson1](src/main/java/lesson1), [lesson2](src/main/java/lesson2), [lesson3](src/main/java/lesson3), [lesson4](src/main/java/lesson4) |
| API-клиенты с Retrofit и Gson | [lesson5](src/main/java/lesson5), [weather](src/main/java/lesson6/homework/weather) |
| Списки, итераторы, множества и отображения | [lesson7](src/main/java/lesson7), [lesson8](src/main/java/lesson8), [lesson9](src/main/java/lesson9), [lesson15](src/main/java/lesson15) |
| Очереди, стеки, исключения и сортировка | [lesson11](src/main/java/lesson11), [lesson12](src/main/java/lesson12), [lesson13](src/main/java/lesson13), [lesson14](src/main/java/lesson14) |
| Producer/consumer и средства многопоточности | [lesson28](src/main/java/lesson28), [lesson34](src/main/java/lesson34), [lesson35](src/main/java/lesson35) |
| JDBC и SQLite | [lesson44](src/main/java/lesson44), [lesson45](src/main/java/lesson45) |
| Тесты JUnit | [src/test/java](src/test/java) |

В [плане курса](docs/course-outline.ru.md) также перечислены темы занятий: Stream API, Spring, Maven и другие. Исходники сгруппированы по урокам в `src/main/java`, тесты — в `src/test/java`.

## Запуск консольного примера

Нужен JDK 18 или новее. В [настройках Maven](pom.xml) указана Java 18 и зависимости JUnit 4, Gson, Retrofit и SQLite JDBC.

```bash
git clone https://github.com/ivan-zamula/java-pro-2022-tel-ran.git
cd java-pro-2022-tel-ran
```

Пример проверки палиндрома использует только стандартную библиотеку Java:

```bash
mkdir -p out
javac -encoding UTF-8 -d out src/main/java/lesson12/PalindromeChecker.java
java -cp out lesson12.PalindromeChecker
```

Результат:

```text
true
false
```

Для примеров с внешними библиотеками откройте `pom.xml` в IntelliJ IDEA как Maven-проект, выберите JDK и дождитесь загрузки зависимостей. Затем запустите нужный класс с `main` или тест JUnit. Примерам с API нужен интернет; JDBC-примеры используют пути к базе данных, заданные в исходниках.
