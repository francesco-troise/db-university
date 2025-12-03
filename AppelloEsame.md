# AppelloEsame

Nome tabella: Appelli

| Campo        | Tipo        | Vincoli                       |
| ------------ | ----------- | ----------------------------- |
| appello_id   | INT         | PRIMARY KEY, NOT NULL         |
| corso_id     | INT         | FOREIGN KEY (Corso), NOT NULL |
| data_appello | DATE        | NOT NULL                      |
| aula         | VARCHAR(50) | NULL                          |
