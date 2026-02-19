# Database Entities

```swift
 ├── ProcessedFile
 ├── EvaluationResult
 └── User
```

- **ProcessedFile** → Tracks processed directories/files with last modified timestamp.  
- **EvaluationResult** → Stores differences found in CSVs.  
- **User** → Stores authentication details (username, password, role).  
- **Reports (logical)** → Generated from `evaluation_results` and `processed_files`.

---

