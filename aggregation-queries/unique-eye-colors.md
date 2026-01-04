## Question
List all unique eye colors present in the users collection.

## Aggregation Pipeline

```js
[
  {
    $group: {
      _id: "$eyeColor"
    }
  }
]
