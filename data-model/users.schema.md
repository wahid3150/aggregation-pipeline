## users collection

This collection stores application users.

### Fields
- _id: ObjectId
- name: String
- email: String
- isActive: Boolean

### Notes
- `isActive` is used to identify currently active users
- This field is commonly used in analytics and reporting queries
- Aggregation pipelines can efficiently count users based on this flag
