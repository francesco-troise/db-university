# IscrizioneAppello

Nome tabella: Iscrizioni_appelli

| Campo       | Tipo                      | Vincoli                              |
| ----------- | ------------------------- | ------------------------------------ |
| studente_id | INT                       | FOREIGN KEY (Studente), NOT NULL     |
| appello_id  | INT                       | FOREIGN KEY (AppelloEsame), NOT NULL |
| voto        | TINYINT                   | NULL                                 |
| PRIMARY KEY | (studente_id, appello_id) | NOT NULL                             |
