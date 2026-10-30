# hello-java


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
