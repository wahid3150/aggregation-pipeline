### Business Question
List the top 5 most common favorite fruits among users.

### What I practiced
- Frequency counting using `$group`
- Ranking results using `$sort`
- Limiting output size using `$limit`

### Key Learning
- Sort direction (`1` vs `-1`) changes business meaning
- MongoDB returns only available groups if fewer exist

### Backend Insight
Ranking queries like this are common in reports,
dashboards, and admin analytics features.