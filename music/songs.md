main table of our music DB

title | duration_in_seconds | release_date | [[artists]] | [[albums]] | [[producers]]

```
CREATE TABLE songs
(
	id SERIAL PRIMARY KEY,
	title TEXT NOT NULL,
	duration_in_seconds INTEGER NOT NULL,
	release_date DATE NOT NULL,
	artists INTEGER[] REFERENCES artists,
	album INTEGER REFERENCES albums,
	producers INTEGER REFERENCES producers
);
```