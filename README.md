# Hello Spring Boot

This is a minimal Spring Boot "Hello, World!" application.

Run locally (PowerShell):

```powershell
mvn spring-boot:run
```

Build jar:

```powershell
mvn -DskipTests package
java -jar target/hello-springboot-0.0.1-SNAPSHOT.jar
```

The application exposes `GET /` which returns `Hello, World!`.

**Docker:** Build and run the app in Docker (PowerShell):

```powershell
mvn -DskipTests package; docker build -t helloworld-app .; docker run --rm -p 8080:8080 helloworld-app
```

Or with Docker Compose:

```powershell
docker-compose up --build
```

The app will be available at `http://localhost:8080/`.
