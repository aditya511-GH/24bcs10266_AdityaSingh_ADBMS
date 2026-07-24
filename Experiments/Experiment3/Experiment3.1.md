Task
Write a query to count the number of students across departments who has scored more than 80 marks.
Alias the count column as 'Dept_HighScore_Count' Your table 'student' has the following columns:
St_id
St_name
Marks
Department
Expected output
┌────────────┬──────────────────────┐
│ department │ Dept_HighScore_Count │
├────────────┼──────────────────────┤
│ Biology    │ 0                    │
│ English    │ 0                    │
│ History    │ 3                    │
│ Math       │ 4                    │
│ Physics    │ 4                    │
└────────────┴──────────────────────┘
solution:

select department, 
count(case when Marks> 80 then 1 else null end) as Dept_HighScore_Count
from student
group by department;
