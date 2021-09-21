[[Passengers]] | Flight data | [[Airlines]] | [[City's]], [[Countries]] | [[City's]], [[Countries]]

```
CREATE TABLE tickets
(
	id SERIAL PRIMARY KEY,
	passenger INTEGER REFERENCES passengers,
	departure TIMESTAMP NOT NULL,
	arrival TIMESTAMP NOT NULL,
	airline INTEGER REFERENCES airlines,
	from_city TEXT REFERENCES cities,
	from_country TEXT REFERENCES countries,
	to_city TEXT REFERENCES cities,
	to_country TEXT REFERENCES countries
);
```