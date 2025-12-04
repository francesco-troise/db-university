# Database Università – Query SQL

-- 1. Selezionare tutti gli studenti nati nel 1990

SELECT \*
FROM students
WHERE YEAR(date_of_birth) = 1990;

///

-- 2. Selezionare tutti i corsi che valgono più di 10 crediti

SELECT \*
FROM courses
WHERE cfu > 10;

///

-- 3. Selezionare tutti gli studenti che hanno più di 30 anni

-- TIMESTAMPDIFF calcola la differenza in anni tra la data di nascita e la data corrente.
SELECT \*
FROM students
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) > 30;

///

-- 4. Selezionare tutti i corsi del primo semestre

SELECT \*
FROM courses
WHERE period = 'I semestre';

///

-- 5. Selezionare tutti gli appelli d'esame nel pomeriggio del 20/06/2020

SELECT \*
FROM exams
WHERE DATE(date) = '2020-06-20'
AND TIME(hour) > '14:00:00';

///

-- 6. Selezionare tutti i corsi di laurea magistrale

SELECT \*
FROM degrees
WHERE `level` = "magistrale";

///

-- 7. Contare quanti dipartimenti ci sono

SELECT COUNT(\*) AS departments
FROM departments;

///

-- 8. Quanti insegnanti non hanno un numero di telefono

SELECT \*
FROM teachers
WHERE phone IS NULL;

///

-- 9. Contare quanti iscritti ci sono stati ogni anno

SELECT
YEAR(enrolment_date) AS anno,
COUNT(\*) AS numero_iscritti
FROM students
GROUP BY YEAR(enrolment_date)
ORDER BY anno;

///

-- 10. Contare gli insegnanti che hanno l'ufficio nello stesso edificio

SELECT
office_address,
COUNT(\*) AS numero_insegnanti
FROM teachers
WHERE office_address IS NOT NULL
GROUP BY office_address
ORDER BY numero_insegnanti DESC;

///

-- 11. Calcolare la media dei voti di ogni appello d'esame

SELECT ROUND(AVG(vote),2) AS decimals, exam_id
FROM exam_student
GROUP BY exam_id;

///

-- 12. Contare quanti corsi di laurea ci sono per ogni dipartimento

SELECT department_id, COUNT(\*) AS count_department
FROM degrees
GROUP BY department_id;
