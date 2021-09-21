holds all users

[[regions]]
```
CREATE TABLE users
(
 id SERIAL PRIMARY KEY
 name TEXT NOT NULL,
 preferred_region INTEGER REFERENCES region ON DELETE CASCADE
);
```