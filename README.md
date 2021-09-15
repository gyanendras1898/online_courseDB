                       An Online Course Enrollment System's Database Design

![Physical model](https://user-images.githubusercontent.com/74998700/133471696-50b08ab1-a497-47fa-ab96-00b8418abd57.PNG)

1.Entire Database Design manages enrolling of students to different online courses from different instructors
whomsoever they prefer.

2.Design composed of total 6 tables here :
(a)Students Table
(b)Enrollments Table
(c)Courses Table
(d)Course Tags Table
(e)Instructors Table
(f)Tags Table

3.Students can buy multiple courses and a single course can be baught by many students so these both has to be interconnected
with many to many relation in design,but this relation is not supported by relational databases.

4.For that,Enrollment table is created ,it works as a link between students table and courses table.

5.Here,tags table can have many values for single course which is violating 1NF.So tags table is created and again there is
many to many relationship between course and tags table.So we link both the table with intermediate table course_tag. 6. According to second normal form, every table should describe only one entity,but in a courses table instructor is a
different entity.So we put instructor into another table and the relation between course and instructor is one to many
as one instructor can teach many course but a course is taught by only one instructor.
