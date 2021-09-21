holds all matches played

[[teams]]
[[referees]]

```
CREATE TABLE matches
(
	id SERIAL PRIMARY KEY,
	date_played DATE NOT NULL,
	teams_played INTEGER[] REFERENCES teams ON DELETE SET NULL,
	referees INTEGER[] REFERENCES referees ON DELETE SET NULL
);
```
