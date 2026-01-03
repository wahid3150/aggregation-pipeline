## Question
How many users are active in the system?

## Thought Process
I wanted to avoid fetching all users and counting them in application code.
Instead, I used MongoDB Aggregation Pipeline to let the database answer this.

## Aggregation Pipeline Used

```js
[
  {
    $match: {
      isActive: true
    }
  },
  {
    $count: "isActive"
  }
]

Result

The aggregation returns an array containing the count of active users:
[
  {
    "activeUsers": 516
  }
]