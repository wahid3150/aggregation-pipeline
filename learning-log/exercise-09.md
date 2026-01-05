## Exercise 09 – Advanced Aggregation with Arrays and Demographics

### Business Question
Among active users, what is the average number of tags per user for each gender?

### What I practiced
- Filtering data using `$match`
- Working with array fields using `$unwind`
- Using multiple `$group` stages
- Aggregating data by demographic fields

### Key Learning
- Arrays must be unwound before per-item aggregation
- Grouping by compound keys enables user-level calculations
- Aggregation pipelines can answer complex analytics questions efficiently

### Backend Insight
Such queries are commonly used in user analytics,
engagement tracking, and reporting dashboards.