main table for outer_space

name | orbital_period_in_years | [[suns]] | [[galaxies]] | moons

```
CREATE TABLE planets
(
 id SERIAL PRIMARY KEY,
 name TEXT NOT NULL,
 orbital_period_in_years FLOAT NOT NULL,
 orbits_around INTEGER REFERENCES suns,
 galaxy INTEGER REFERENCES galaxies,
 moons TEXT[] 
);
```