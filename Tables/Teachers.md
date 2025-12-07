# Table: Teachers

Entity: Teacher

## Description

Elenco dei docenti dell’università.

---

## Columns

| Column         | Type         | Constraints              | Description                         |
| -------------- | ------------ | ------------------------ | ----------------------------------- |
| id             | SMALLINT     | PK, AI, UNIQUE, NOT NULL | Identificativo docente.             |
| name           | VARCHAR(35)  | NOT NULL                 | Nome.                               |
| surname        | VARCHAR(35)  | NOT NULL                 | Cognome.                            |
| phone          | VARCHAR(15)  | UNIQUE, NULL             | Numero di telefono.                 |
| email          | VARCHAR(100) | UNIQUE, NULL             | Email istituzionale.                |
| office_address | VARCHAR(100) | UNIQUE, NULL             | Indirizzo dell’ufficio del docente. |
| office_number  | TINYINT      | UNIQUE, NOT NULL         | Numero dell’ufficio.                |

---
