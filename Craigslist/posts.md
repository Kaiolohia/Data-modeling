Main table for craigslist, holds all posts

[[users]]
[[regions]]
[[catagories]]

```
CREATE TABLE posts
(
 id SERIAL PRIMARY KEY,
 title TEXT NOT NULL,
 poster INTEGER REFERENCES users ON DELETE CASCADE,
 location TEXT NOT NULL,
 region INTEGER REFERENCES region ON DELETE CASCADE,
 category INTEGER REFERENCES categories ON DELETE CASCADE,
);
```