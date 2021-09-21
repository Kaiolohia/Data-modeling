Holds all registered referees

[[matches]]

```
CREATE TABLE referees
(
	id SERIAL PRIMARY KEY,
	name TEXT NOT NULL,
	games_refd INTEGER[] REFERENCES matches ON DELETE CASCADE
);
```