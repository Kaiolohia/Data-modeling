Holds all registered players and their team
[[teams]]

```
CREATE TABLE players
(
	id SERIAL PRIMARY KEY,
	name TEXT NOT NULL
	team INTEGER REFERENCES teams ON DELETE CASCADE
);
```