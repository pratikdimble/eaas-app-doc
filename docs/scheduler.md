```markdown
# Scheduler

```
Scheduler (@Scheduled)<br>
 └── Runs every minute<br>
      └── Calls readMultipleCSVs(true)
```

- Configured with `@Scheduled(cron = "0 * * * * *")`.  
- Runs batch evaluation every minute.  
- Logs processed directories and differences found.  
- Batch saves processed file metadata and evaluation results.

---

## Related Pages
- [Home](index.md)
- [Database Entities](database.md)
```

---
