holds all of the enrolled patients
```
CREATE TABLE patients
(
 id SERIAL PRIMARY KEY,
 name TEXT NOT NULL,
 diseases TEXT[] NOT NULL,
 doctors INTEGER[] REFERENCES doctors ON DELETE CASCADE
);
```