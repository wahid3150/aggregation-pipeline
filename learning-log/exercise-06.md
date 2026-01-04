## Exercise 06 – Finding Unique Values

### Business Question
List all unique eye colors present in the collection.

### What I practiced
- Using `$group` to find distinct values
- Aggregating categorical data without accumulators

### Key Learning
- `$group` can be used purely for uniqueness
- MongoDB returns one document per unique value

### Backend Insight
This pattern is useful for building filters
and dynamic UI options based on stored data.
