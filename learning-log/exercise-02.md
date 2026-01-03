## Exercise 2 – Aggregation with `$group` and  `$avg`

### What I practiced
- Used `$group` to aggregate across all documents
- Calculated average value using `$avg`

### Business Question
What is the average age of all users?

### Key Learning
- `$group` can be used without a grouping key using `_id: null`
- Aggregation pipelines are well-suited for analytics use cases

### Backend Insight
Database-level aggregation is more scalable than
calculating averages inside application logic.
