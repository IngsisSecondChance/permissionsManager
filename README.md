# Ingsis Microservices

Este repositorio agrupa los tres microservicios desarrollados en la práctica de Ingeniería de Sistemas (4to año Ing. Informática).

## 📐 Arquitectura
- Diagrama de componentes: [link o imagen aquí]
- Cada microservicio está contenido como submódulo en este repo:
    - [Permissions Manager](./permissionsManager)
    - [Snippet Manager](./snippetManager)
    - [PrintScript Manager](./printScriptManager)

## 🖥️ Microservicios
### Permissions Manager
- Puerto: `8083`
- Base de datos: `permsdb`
- Carpeta: [`permissionsManager`](./permissionsManager)

### Snippet Manager
- Puerto: `8081`
- Base de datos: `snippetdb`
- Carpeta: [`snippetManager`](./snippetManager)

### PrintScript Manager
- Puerto: `8082`
- Base de datos: `printdb`
- Carpeta: [`printScriptManager`](./printScriptManager)

## ⚙️ Tecnologías
- **Spring Boot 3.x**
- **Gradle Kotlin DSL**
- **PostgreSQL** con **Testcontainers** en los tests
- **Spotless** (formatter), **Checkstyle** (linter), **JaCoCo** (coverage)
- **GitHub Actions** para CI/CD

## 🚀 Cómo correr local
```bash
# Clonar con submódulos
git clone --recursive <url-repo>

# Entrar en un servicio
cd permissionsManager

# Correr tests
./gradlew clean test

# Correr la app local
./gradlew bootRun