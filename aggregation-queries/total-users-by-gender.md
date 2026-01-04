## Question
Find the total number of male and female users.

## Aggregation Pipeline

```js
[
  {
    $group: {
      _id: "$gender",
      genderCount: { $sum: 1 }
    }
  }
]
