### Cyberchase Part 2 - Proof of Effort
-- 9/8/25 ncruz
--cyberchase part 2

--problem category
--students (name, age, grade, score)
--problem question 


### Tool Used
ChatGPT (GPT-4)

### Problem 1
Write a query to find the average grade for all students in the Math course.

### Summary of Learning
- Use AVG(grade)
- check tables names
- study AS

### Sample Query Attempt
``` SELECT AVERAGE "grade" FROM "math" ```

### Problem 2
Write a query to find the names of students who passed AND had a grade greater than 85
### Summary of Learning
- heck name of table should be "student"
- AND passed = TRUE 


### Sample Query Attempt
``` SELECT "names" FROM "students" WHERE "grade" > 85 ; ```


### Problem 3
Write a query to find the total number of students who are taking History and did not pass.

### Summary of Learning
- replace select with SELECT COUNT(*) no space, 
- Not IN, should be WHERE course = 'History"



### Sample Query Attempt
``` SELECT COUNT (*) "students" IN "history" WHERE FALSE ```

### Problem 4
Find the average grade of students who passed, grouped by course


### Summary of Learning
- Issues with no quotes for grade , learned GROUP BY course
- Not IN, should be WHERE course = 'History"



### Sample Query Attempt
``` SELECT AVERAGE "grade" FROM "student" WHERE "passed" AND "grouped_by_course" ;```

### Problem 5
Write a query to get the average grade of students who passed (all courses combined).


### Summary of Learning
- Issues with no quotes for grade , learned GROUP BY course
- Not IN, should be WHERE course = 'History"



### Sample Query Attempt
``` SELECT AVG(grade) AS avg_grade FROM students WHERE passed = TRUE;```
