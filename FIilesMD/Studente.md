# Studente

Nome tabella: studenti

| Campo           | Tipo         | Vincoli                             |
| --------------- | ------------ | ----------------------------------- |
| studente_id     | INT          | PRIMARY KEY, NOT NULL               |
| corso_laurea_id | INT          | FOREIGN KEY (CorsoLaurea), NOT NULL |
| nome            | VARCHAR(100) | NOT NULL                            |
| cognome         | VARCHAR(100) | NOT NULL                            |
| matricola       | VARCHAR(20)  | UNIQUE, NOT NULL                    |
