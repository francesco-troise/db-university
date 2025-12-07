# Table: Courses_Teachers

Entity: Course_Teacher (Bridge Table)

## Description

Tabella ponte che modella la relazione molti-a-molti tra corsi e docenti.

---

## Columns

| Column     | Type     | Constraints  | Description        |
| ---------- | -------- | ------------ | ------------------ |
| course_id  | SMALLINT | FK, NOT NULL | Corso insegnato.   |
| teacher_id | SMALLINT | FK, NOT NULL | Docente assegnato. |

---

## Notes

- La PK potrebbe essere composta: `(course_id, teacher_id)`.
