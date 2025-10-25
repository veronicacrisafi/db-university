## table: university

- id
- departments
- courses
- teachers
- exam_appeals
- students
- student_exam_enrollments
- vote

### table: departments

- id (PK)
- department_name

### table: courses

- id (PK)
- department_id (FK)
- course_name

### table: teachers

- id (PK)
- name
- last_name
- course_id (FK)

### table: exams_appeals

- id (PK)
- teacher_id (FK)
- course_id (FK)
- exam_date
- exam_time
- exam_name
- exam_location

### table: students

- id (PK)
- course_id (FK)
- name
- last_name
- date_of_birth
- student_number
- mail
- phone_number
- academic_year
- status (active/retired/graduated)

### table: student_exam_enrollments

- id (PK)
- student_id (FK)
- exam_appeal_id (FK)
- enrollment_date
- status (registered/withdrawn/present)

### table : votes

- id (PK)
- student_id
