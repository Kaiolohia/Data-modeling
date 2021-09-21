Holds the employed doctors
```
CREATE TABLE doctors
(
 id SERIAL PRIMARY KEY,
 name TEXT NOT NULL,
 patients INTEGER REFERENCES patients ON DELETE CASCADE
);
```