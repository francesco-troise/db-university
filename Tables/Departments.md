# Table: Departments

Entity: Department

## Description

Rappresenta i dipartimenti universitari. Ogni dipartimento gestisce corsi di laurea, personale e strutture associate.

---

## Columns

| Column             | Type         | Constraints              | Description                                    |
| ------------------ | ------------ | ------------------------ | ---------------------------------------------- |
| id                 | SMALLINT     | PK, AI, UNIQUE, NOT NULL | Identificativo univoco del dipartimento.       |
| name               | VARCHAR(50)  | NOT NULL, UNIQUE         | Nome del dipartimento (es. “Ingegneria”).      |
| address            | VARCHAR(100) | NOT NULL                 | Indirizzo fisico del dipartimento.             |
| phone              | VARCHAR(20)  | NOT NULL, UNIQUE         | Numero di telefono ufficiale.                  |
| email              | VARCHAR(100) | NOT NULL, UNIQUE         | Email istituzionale.                           |
| website            | VARCHAR(50)  | NULL                     | Sito web ufficiale.                            |
| head_of_department | VARCHAR(50)  | NULL                     | Nome e cognome del direttore del dipartimento. |

---
