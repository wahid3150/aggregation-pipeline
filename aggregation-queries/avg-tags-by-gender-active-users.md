## Question
Among active users, what is the average number of tags per user for each gender?

## Aggregation Pipeline

```js
[
  {
    $match: {
      isActive: true
    }
  },
  {
    $unwind: "$tags"
  },
  {
    $group: {
      _id: {
        userId: "$_id",
        gender: "$gender"
      },
      numberOfTags: { $sum: 1 }
    }
  },
  {
    $group: {
      _id: "$_id.gender",
      averageNumberOfTags: {
        $avg: "$numberOfTags"
      }
    }
  }
]
