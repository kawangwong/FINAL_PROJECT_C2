Application:
Educational web app that allows students to take quizlet like exams, allow students to provide feedback to the instructor in general via email. The application will perform an action that will alert the teacher of any new exams that were taken and completed by the student.

Detailed explanation:
Student will login (maybe) and then choose an exam to take.  Student puts their name in. The exam is taken and completed. That exam score will then be sent to the teacher. Second function is to send an email to the teacher in general. Last function is for teacher to be allowed to edit the exam or maybe even make a new one.

Front end:
Html css js to make UI for user to be seamless and able to interact and submit information through get and posts requests.
Backend:
Using python flask, specifically SQL based db so we can use sqlalchemy. We also want to consider implementing a login for user as well as teacher and have it encrypted. Last, we use flask mail to set up mailing server thing for sending emails to teacher.

How we connect it. Unclear, depending on the template or home built application, we will use SQLITE RDS. With the database approach, we only want to record the final grade of each exam, so we doing break the schema as it is Relational. A second table exists as a means to store user credentials if it is implemented. Grading. How do we grade? If using template, the grading will use doc file reads and post requests. If no template, python, maybe pandas to pull data, and assert values from another file. This could get messy if we create a teacher account to add or remove quizzes and also questions.
Limitations:
SQL schema is the limit, so keep questions at set value of x many questions.
Storing values in plain text such as answers and question keys. How do we fix this if not using template or even with template.
