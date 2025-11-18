# My-Projects
This is my first repository.
CREATE database school;

CREATE TABLE stu(
	student_id int primary key,
	name varchar(50),
	age int,
	grade int
	);

	CREATE TABLE course(
		course_id int primary key,
		course_name varchar(50)
		);

	CREATE TABLE enrollments(
		student_id int,
		course_id int,
		PRIMARY KEY (student_id, course_id),
		FOREIGN KEY (student_id) REFERENCES Stu(student_id),
		FOREIGN KEY (course_id) REFERENCES Course(course_id)
		);
