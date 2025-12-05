# CorsoLaurea

Nome_tabella: corsi_laurea

| Campo           | Tipo         | Vincoli                              |
| --------------- | ------------ | ------------------------------------ |
| corso_laurea_id | INT          | PRIMARY KEY, NOT NULL                |
| dipartimento_id | INT          | FOREIGN KEY (Dipartimento), NOT NULL |
| nome            | VARCHAR(150) | NOT NULL                             |
| livello         | VARCHAR(50)  | NULL                                 |
