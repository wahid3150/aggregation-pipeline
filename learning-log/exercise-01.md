## Exercise 01 – MongoDB Aggregation Pipeline (Basics)

### What I did
- Installed MongoDB VS Code Extension
- Inserted data into three collections:
  - users
  - books
  - authors
- Explored aggregation pipeline in both:
  - Stage builder
  - Text mode

### Business Question
How many users are currently active?

### Aggregation Used
- $match to filter active users
- $count to calculate total active users

### Result
Total active users: 516

### Key Backend Learning
- Aggregation pipelines allow the database to answer business questions directly
- This avoids fetching unnecessary documents into backend code
- Improves performance and scalability
