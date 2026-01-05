## Exercise 08 – Combining Filters with Analytics

### Business Question
Among active users, which 3 countries have the highest average age?

### What I practiced
- Filtering documents using `$match`
- Aggregating data on nested fields
- Calculating averages with `$avg`
- Ranking results using `$sort`

### Key Learning
- Applying `$match` early improves query efficiency
- MongoDB can aggregate deeply nested fields directly
- Multiple metrics can be calculated in a single `$group`

### Backend Insight
This aggregation pattern is useful for demographic analysis,
market segmentation, and admin reporting features.