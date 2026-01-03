## authors collection

This collection stores authors information.

### Fields
- _id: Number
- name: String
- birth_year: Number

### Notes
- `_id` is referenced in books.author_id
- This allows relational-style aggregation using $lookup
