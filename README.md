# Java Pro (Tel-Ran, 2022)

[English](README.md) | [Русский](README.ru.md)

Java exercises and homework from the Tel-Ran professional course. The repository includes custom collections, object-oriented models, API clients, concurrent code, database examples and unit tests.

## Explore the code

| Topic | Examples |
| --- | --- |
| Classes, inheritance, enums and interfaces | [lesson1](src/main/java/lesson1), [lesson2](src/main/java/lesson2), [lesson3](src/main/java/lesson3), [lesson4](src/main/java/lesson4) |
| API clients with Retrofit and Gson | [lesson5](src/main/java/lesson5), [weather](src/main/java/lesson6/homework/weather) |
| Lists, iterators, sets and maps | [lesson7](src/main/java/lesson7), [lesson8](src/main/java/lesson8), [lesson9](src/main/java/lesson9), [lesson15](src/main/java/lesson15) |
| Queues, stacks, exceptions and sorting | [lesson11](src/main/java/lesson11), [lesson12](src/main/java/lesson12), [lesson13](src/main/java/lesson13), [lesson14](src/main/java/lesson14) |
| Producer/consumer and concurrent utilities | [lesson28](src/main/java/lesson28), [lesson34](src/main/java/lesson34), [lesson35](src/main/java/lesson35) |
| JDBC and SQLite | [lesson44](src/main/java/lesson44), [lesson45](src/main/java/lesson45) |
| JUnit tests | [src/test/java](src/test/java) |

The [course outline](docs/course-outline.md) also lists topics covered in class, including streams, Spring and Maven. Source examples are grouped by lesson under `src/main/java`; tests are under `src/test/java`.

## Run a console example

Use JDK 18 or newer. The [Maven configuration](pom.xml) targets Java 18 and lists JUnit 4, Gson, Retrofit and SQLite JDBC dependencies.

```bash
git clone https://github.com/ivan-zamula/java-pro-2022-tel-ran.git
cd java-pro-2022-tel-ran
```

This palindrome example uses only the standard Java library:

```bash
mkdir -p out
javac -encoding UTF-8 -d out src/main/java/lesson12/PalindromeChecker.java
java -cp out lesson12.PalindromeChecker
```

Output:

```text
true
false
```

To explore examples with external libraries in IntelliJ IDEA, open `pom.xml` as a Maven project, select your JDK and let Maven download the dependencies. Run the chosen `main` class or JUnit test. API examples need internet access; JDBC examples use the database paths set in their source files.
