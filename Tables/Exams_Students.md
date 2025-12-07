# Table: Exams_Students

Entity: Exam_Student (Bridge Table)

## Description

Registra gli studenti iscritti agli appelli e il voto ottenuto.

---

## Columns

| Column     | Type     | Constraints  | Description        |
| ---------- | -------- | ------------ | ------------------ |
| student_id | INT      | FK, NOT NULL | Studente iscritto. |
| exam_id    | SMALLINT | FK, NOT NULL | Appello d’esame.   |
| voto       | TINYINT  | NOT NULL     | Voto ottenuto.     |

---

## Notes

- La PK potrebbe essere copmosta: `(student_id, exam_id)`.
