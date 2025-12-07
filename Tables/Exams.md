# Table: Exams

Entity: Exam

## Description

Appelli d'esame associati ai singoli corsi.

---

## Columns

| Column    | Type         | Constraints              | Description              |
| --------- | ------------ | ------------------------ | ------------------------ |
| id        | SMALLINT     | PK, AI, UNIQUE, NOT NULL | Identificativo esame.    |
| course_id | SMALLINT     | FK, NOT NULL             | Riferimento al corso.    |
| date      | DATE         | NULL                     | Data dell’appello.       |
| hour      | TIME         | NULL                     | Orario dell’esame.       |
| location  | VARCHAR(100) | NULL                     | Luogo (es. aula).        |
| address   | VARCHAR(100) | NULL                     | Indirizzo dell’edificio. |

---
