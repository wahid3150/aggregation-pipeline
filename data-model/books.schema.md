## books collection

This collection stores books data.

### Fields
- _id: Number
- title: String
- author_id: Number
- genre: String

### Notes
- `author_id` references the authors collection
- This structure supports future $lookup aggregation
