# Table: Courses

Entity: Course

## Description

Raccolta dei singoli insegnamenti appartenenti ai corsi di laurea.

---

## Columns

| Column      | Type        | Constraints              | Description                      |
| ----------- | ----------- | ------------------------ | -------------------------------- |
| id          | SMALLINT    | PK, AI, UNIQUE, NOT NULL | Identificativo del corso.        |
| degree_id   | SMALLINT    | FK, NOT NULL             | Corso di laurea di appartenenza. |
| name        | VARCHAR(50) | UNIQUE, NOT NULL         | Nome dell’insegnamento.          |
| description | TEXT        | NULL                     | Descrizione estesa del corso.    |
| period      | VARCHAR(15) | NOT NULL                 | Periodo (es. primo semestre).    |
| year        | TINYINT     | NOT NULL                 | Anno di erogazione.              |
| cfu         | TINYINT     | NOT NULL                 | Crediti formativi (CFU).         |
| website     | VARCHAR(50) | NULL                     | Sito del corso.                  |

---
