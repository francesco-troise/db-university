# Insegnante

Nome tabella: insegnanti

| Campo         | Tipo         | Vincoli               |
| ------------- | ------------ | --------------------- |
| insegnante_id | INT          | PRIMARY KEY, NOT NULL |
| nome          | VARCHAR(100) | NOT NULL              |
| cognome       | VARCHAR(100) | NOT NULL              |
| email         | VARCHAR(150) | UNIQUE, NULL          |
