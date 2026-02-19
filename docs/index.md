```markdown
# Evaluation Service API Portfolio

## Overview
The **Evaluation Service API** is a Spring Boot application that:
- Evaluates CSV files in **batch** or **online** mode.
- Detects differences between records using header‑based parsing.
- Persists results into the database (`evaluation_results`, `processed_files`).
- Exports summaries and detailed reports as CSV.
- Provides JSON reports for dashboards and integrations.
- Supports authentication with JWT (`users` table).
- Runs scheduled jobs to automate batch evaluation.

---

## Architecture

```
User / Scheduler<br>
       │<br>
       ▼<br>
Controllers<br>
 ├── EvaluationController<br>
 ├── ExportController<br>
 ├── AuthController<br>
 └── ReportController<br>
       │<br>
       ▼<br>
Service Layer<br>
 ├── EvaluationService<br>
 ├── JwtService<br>
 └── ReportService<br>
       │<br>
       ▼<br>
Utilities<br>
 └── CsvUtils<br>
       │<br>
       ▼<br>
Database<br>
 ├── processed_files<br>
 ├── evaluation_results<br>
 └── users
```

---

## Explore More
- [Controllers](controllers.md)
- [Service Layer](services.md)
- [Utilities](utilities.md)
- [Database Entities](database.md)
- [Scheduler](scheduler.md)

---

## Quick Start Guide

### Prerequisites
- Java 17+
- Maven 3.8+
- A running database (configure in `application.properties`)

### Setup
```bash
git clone https://github.com/pratikdimble/evaluation-service-api.git
cd evaluation-service-api
git checkout development
```

### Build & Run
```bash
mvn clean install
mvn spring-boot:run
```

### Access Swagger UI
```
http://localhost:8080/swagger-ui/index.html
```
```

## Related Pages
- [Home](index.md)
- [Service Layer](services.md)
```
