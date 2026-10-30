# hello-java

![Java CI](https://github.com/Evgeny65ok/hello-java/actions/workflows/ci.yml/badge.svg)

<img width="1720" height="442" alt="image" src="https://github.com/user-attachments/assets/57049a6f-2abb-4e58-ae2f-3a78e532b3c4" />




Пример Java-приложения с Maven, JUnit 5, Docker (multi-stage) и CI на GitHub Actions.

## Что внутри

- `pom.xml` — конфиг Maven с JUnit 5 и Shade Plugin
- `src/main/java/Hello.java` — приложение
- `src/test/java/HelloTest.java` — тесты
- `Dockerfile` — двухэтапная сборка (Maven → JRE alpine)
- `.github/workflows/ci.yml` — пайплайн CI

## Проверка локально

```bash
docker build -t hello-java .
docker run --rm hello-java
```

Ожидаемый вывод:

```
Hello from Java in Docker! ☕🐳
Java version: 17.0.x
OS: Linux
```
