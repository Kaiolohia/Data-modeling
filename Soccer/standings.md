holds league data relating to teams

[[teams]]
[[leagues]]

```
CREATE TABLE standings
(
 id SERIAL PRIMARY KEY,
 league INTEGER REFERENCES leagues ON DELETE CASCADE,
 team INTEGER REFERENCES teams ON DELETE CASCADE,
 standing INTEGER NOT NULL
);
```