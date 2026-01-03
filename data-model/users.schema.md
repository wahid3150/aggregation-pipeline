## users collection

This collection stores application users along with profile,
activity status, and company-related metadata.

### Fields

- _id: ObjectId  
  Unique identifier for each user.

- index: Number  
  Dataset index (used for reference in sample data).

- name: String  
  Full name of the user.

- isActive: Boolean  
  Indicates whether the user is currently active.
  Commonly used in analytics and filtering queries.

- registered: Date  
  The date when the user registered.

- age: Number  
  Age of the user.
  Used in aggregation queries such as average, min, max age.

- gender: String  
  Gender of the user.

- eyeColor: String  
  Eye color attribute.

- favoriteFruit: String  
  User’s preferred fruit (categorical data).

- company: Object  
  Embedded company information.
  
  - title: String  
    Company name.

  - email: String  
    Company contact email.

  - phone: String  
    Company contact phone number.

  - location: Object  
    Company location details.
    
    - country: String  
    - address: String  

- tags: Array<String>  
  List of tags associated with the user.
  Useful for filtering and array-based aggregation queries.

---

### Notes

- This schema supports:
  - `$match` on `isActive`, `gender`, `eyeColor`
  - `$group` on `age`, `favoriteFruit`, `company.location.country`
  - `$avg`, `$min`, `$max` on numeric fields like `age`
  - `$unwind` and `$group` on `tags`
- Embedded company data avoids the need for joins in most assume cases
- Designed for analytics-style aggregation pipelines
