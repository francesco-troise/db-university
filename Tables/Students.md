# Table: Students

Entity: Student

## Description

Rappresenta gli studenti iscritti all’università.

---

## Columns

| Column              | Type        | Constraints              | Description                  |
| ------------------- | ----------- | ------------------------ | ---------------------------- |
| id                  | INT         | PK, AI, UNIQUE, NOT NULL | Identificativo studente.     |
| degree_id           | SMALLINT    | FK, NOT NULL             | Corso di laurea frequentato. |
| name                | VARCHAR(35) | NOT NULL                 | Nome.                        |
| surname             | VARCHAR(35) | NOT NULL                 | Cognome.                     |
| date_of_birth       | DATE        | NULL                     | Data di nascita.             |
| fiscal_code         | CHAR(16)    | NOT NULL                 | Codice fiscale.              |
| enrolment_date      | DATE        | NOT NULL                 | Data di immatricolazione.    |
| registration_number | INT         | NOT NULL                 | Numero di matricola.         |
| email               | VARCHAR(50) | NOT NULL                 | Email istituzionale.         |

---
