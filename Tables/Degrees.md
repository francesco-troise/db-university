# Table: Degrees

Entity: Degree

## Description

Definisce i corsi di laurea offerti dai vari dipartimenti.

---

## Columns

| Column        | Type         | Constraints              | Description                                     |
| ------------- | ------------ | ------------------------ | ----------------------------------------------- |
| id            | SMALLINT     | PK, AI, UNIQUE, NOT NULL | Identificativo univoco del corso di laurea.     |
| department_id | SMALLINT     | FK, NOT NULL             | Riferimento al dipartimento che offre il corso. |
| name          | VARCHAR(50)  | UNIQUE, NOT NULL         | Nome del corso di laurea.                       |
| level         | VARCHAR(30)  | NOT NULL                 | Livello (es. Triennale, Magistrale).            |
| address       | VARCHAR(100) | NOT NULL                 | Indirizzo della segreteria del corso.           |
| email         | VARCHAR(100) | UNIQUE, NOT NULL         | Email ufficiale del corso.                      |
| website       | VARCHAR(50)  | NULL                     | Sito web del corso.                             |

---
