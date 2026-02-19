# Service Layer

## EvaluationService
- `readMultipleCSVs(Boolean isBatch)` → Parallel directory processing, batch persistence.
- `processDirectory(...)` → Skips unchanged directories, parses CSV, adds `ProcessedFile`.
- `parseCsv(...)` → Builds header index, detects differences, batch saves `EvaluationResult`.

## JwtService
- Generates and validates JWT tokens for authentication.

## ReportService
- Aggregates results from `evaluation_results` and `processed_files` for reporting endpoints.

---

