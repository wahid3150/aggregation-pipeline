## Question
Among active users, which 3 countries have the highest average age?

## Aggregation Pipeline

```js
[
  {
    $match: {
      isActive: true
    }
  },
  {
    $group: {
      _id: "$company.location.country",
      averageAge: { $avg: "$age" },
      totalUsers: { $sum: 1 }
    }
  },
  {
    $sort: {
      averageAge: -1
    }
  },
  {
    $limit: 3
  }
]
