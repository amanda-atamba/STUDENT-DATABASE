# STUDENT-DATABASE
CREATE TABLE students (
  name VARCHAR(255),
  hobby VARCHAR(255),
  admissionnumber INT
  );
SELECT * FROM students;

INSERT INTO students (name,hobby,admissionnumber)
VALUES
  ('Amanda','BasketBall','184167'),
  ('Natasha','VollyBall','190552'),
  ('Audrey','Music','122444');
SELECT * FROM students;
SELECT name,hobby FROM students;

ALTER TABLE students
ADD faculty VARCHAR(255);
SELECT * FROM students;

UPDATE students
SET faculty = 'SCES'
WHERE name = 'Amanda';
SELECT * FROM students;

UPDATE students
SET faculty = 'SCES'
WHERE name = 'Natasha';
SELECT * FROM students;

UPDATE students
SET faculty = 'MEDICINE'
WHERE name = 'Audrey';
SELECT * FROM students;

ALTER TABLE students
DROP COLUMN faculty;
SELECT * FROM students;

DELETE FROM students
WHERE name ='Amanda';
SELECT * FROM students;
