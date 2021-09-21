holds all leagues

```
CREATE TABLES leagues
(
 id SERIAL PRIMARY KEY,
 name TEXT NOT NULL,
 start_date DATE NOT NULL,
 end_date DATE NOT NULL
);
```