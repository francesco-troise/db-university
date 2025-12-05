# Corso

Nome tabella:Corsi

| Campo           | Tipo         | Vincoli                             |
| --------------- | ------------ | ----------------------------------- |
| corso_id        | INT          | PRIMARY KEY, NOT NULL               |
| corso_laurea_id | INT          | FOREIGN KEY (CorsoLaurea), NOT NULL |
| nome            | VARCHAR(150) | NOT NULL                            |
| cfu             | INT          | NOT NULL                            |
