# Controllers

## EvaluationController
```java
 ├── GET /evaluate?isBatch=true
 ├── GET /evaluate/internal?isBatch=true
 ├── GET /evaluate/export-csv?isBatch=true
 └── GET /evaluate/model-detail/{model}?isBatch=true
```

## ExportController
```java
 ├── GET /export/summary?isBatch=true
 └── GET /export/detail/{model}?isBatch=true
```

## AuthController
```java
 ├── POST /auth/register
 └── POST /auth/login
```

## ReportController
```java
 ├── GET /report/summary?isBatch=true
 ├── GET /report/detail/{model}?isBatch=true
 └── GET /report/all?isBatch=true
```
