## Fetching, Inserting, Deleting and Updating Rows
Fetch the row from User table based on Id and Password.
```
SELECT * FROM notemanagement.user
WHERE user_id = '1' AND user_password = 'xyz';
```
Fetch all the rows from Note table based on the field note_creation_date.
```
SELECT * FROM notemanagement.note
WHERE note_creation_date='2021-02-27';
```
Fetch all the Categories created after the particular Date.
```
SELECT * FROM notemanagement.category
WHERE category_creation_date > '2021-02-25';
```
Fetch all the Note ID from UserNote table for a given User.
```
SELECT note_id FROM notemanagement.usernote 
WHERE user_id='1';
```
Write Update query to modify particular Note for the given note Id.
```
UPDATE notemanagement.note
SET note_title='Hi There'
WHERE note_id='1';
```
Fetch all the Notes from the Note table by a particular User.
```
SELECT * FROM notemanagement.note 
WHERE user_id='1';
```
Fetch all the Notes from the Note table by a particular User.
```
SELECT * FROM notemanagement.note AS t1
INNER JOIN notemanagement.usernote AS t2
ON t1.note_id = t2.note_id
WHERE t2.user_id='1';
```
Fetch all the Notes from the Note table for a particular Category.
```
SELECT * FROM notemanagement.note AS t1
INNER JOIN notemanagement.notecategory AS t2
ON t1.note_id = t2.note_id
WHERE t2.category_id='1';
```
Fetch all the reminder details for a given note id.
```
SELECT * FROM notemanagement.reminder AS t1
INNER JOIN notemanagement.notereminder AS t2
ON t1.reminder_id = t2.reminder_id
WHERE t2.note_id='1';
```
Fetch the reminder details for a given reminder id.
```
SELECT * FROM notemanagement.reminder
WHERE reminder_id='1';
```
Write a query to create a new Note from particular User (Use Note and UserNote tables - insert statement)
```
INSERT INTO notemanagement.note (note_title, note_content, note_status, note_creation_date)
VALUES ('new note', 'hello world !!', 'completed', '2021-02-28');
INSERT INTO notemanagement.usernote (user_id, note_id) 
VALUES (last_insert_id(), '1');
```
Write a query to create a new Note from particular User to particular Category(Use Note and NoteCategory tables - insert statement)
```
```
Write a query to set a reminder for a particular note (Use Reminder and NoteReminder tables - insert statement)
```
```
Write a query to delete particular Note added by a User(Note and UserNote tables - delete statement)
```
```
Write a query to delete particular Note from particular Category(Note and NoteCategory tables - delete statement)
```
```
Create a trigger to delete all matching records from UserNote, NoteReminder and NoteCategory table when :
* A particular note is deleted from Note table (all the matching records from UserNote, NoteReminder and NoteCategory should be removed automatically)
```
```
* A particular user is deleted from User table (all the matching notes should be removed automatically)
```
```