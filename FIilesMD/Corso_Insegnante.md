# Corso_Insegnante

Nome tabella: Pivot_corso_insegnante

| Campo         | Tipo                      | Vincoli                            |
| ------------- | ------------------------- | ---------------------------------- |
| corso_id      | INT                       | FOREIGN KEY (Corso), NOT NULL      |
| insegnante_id | INT                       | FOREIGN KEY (Insegnante), NOT NULL |
| PRIMARY KEY   | (corso_id, insegnante_id) | NOT NULL                           |
