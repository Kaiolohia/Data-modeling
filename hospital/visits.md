Main table for the hospital, holds all of the doctors and patients that have ever gone through the hospital.

visited | [[patients]] | [[doctors]] | reason_for_visit
```
CREATE TABLE doctors
(
 id SERIAL PRIMARY KEY,
 visited TIMESTAMP NOT NULL,
 patient INTEGER REFERENCES patients ON DELETE SET NULL,
 doctor INTEGER REFERENCES doctors ON DELETE SET NULL,
 reason_for_visit TEXT NOT NULL
);
```