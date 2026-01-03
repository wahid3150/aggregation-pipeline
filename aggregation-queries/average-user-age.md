## Question
What is the average age of all users?

## Aggregation Pipeline Used

```js
[
  {
    $group: {
      _id: null,
      averageAge: {
        $avg: "$age"
      }
    }
  }
]