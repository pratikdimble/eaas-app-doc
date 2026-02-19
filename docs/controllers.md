```markdown 
# Controllers
```
## EvaluationController
```
 ├── GET /evaluate?isBatch=true<br>
 ├── GET /evaluate/internal?isBatch=true<br>
 ├── GET /evaluate/export-csv?isBatch=true<br>
 └── GET /evaluate/model-detail/{model}?isBatch=true
```

## ExportController
```
 ├── GET /export/summary?isBatch=true<br>
 └── GET /export/detail/{model}?isBatch=true
```

## AuthController
```
 ├── POST /auth/register<br>
 └── POST /auth/login
```

## ReportController
```
 ├── GET /report/summary?isBatch=true<br>
 ├── GET /report/detail/{model}?isBatch=true<br>
 └── GET /report/all?isBatch=true
```
