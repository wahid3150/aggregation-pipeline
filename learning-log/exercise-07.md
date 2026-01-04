## Exercise 07 – Aggregation with Arrays

### Business Question
What is the average number of tags per user?

### What I practiced
- Using `$unwind` to work with array fields
- Multi-stage grouping
- Calculating averages across grouped data

### Key Learning
- Arrays must be unwound before aggregation
- Multiple `$group` stages can be chained for complex analytics

### Backend Insight
This pattern is commonly used in analytics,
recommendation systems, and user profiling.