## Adding Rows

```
INSERT INTO notemanagement.user (user_name, user_added_date, user_password, user_mobile) 
VALUES ('lari', '2021-02-26', 'xyz', '9089604511');
INSERT INTO notemanagement.user (user_name, user_added_date, user_password, user_mobile) 
VALUES ('ida', '2021-02-22', 'pqrs', '7005646464');
INSERT INTO notemanagement.user (user_name, user_added_date, user_password, user_mobile) 
VALUES ('michi', '2021-03-14', 'lmn', '7005645343');
```

```
INSERT INTO notemanagement.note (note_title, note_content, note_status, note_creation_date) 
VALUES ('hello', 'world', 'pending', '2021-02-27');
INSERT INTO notemanagement.note (note_title, note_content, note_status, note_creation_date) 
VALUES ('hello hello', 'world !!', 'pending', '2021-02-27');
INSERT INTO notemanagement.note (note_title, note_content, note_status, note_creation_date) 
VALUES ('to be noted', 'hello world', 'completed', '2021-03-09');
```

```
INSERT INTO notemanagement.category (category_name, category_descr, category_creation_date) 
VALUES ('shopping', 'shopping list notes', '2021-02-26');
INSERT INTO notemanagement.category (category_name, category_descr, category_creation_date) 
VALUES ('todo', 'list of things to be done', '2021-02-26');
```

```
INSERT INTO notemanagement.reminder (reminder_name, reminder_descr, reminder_type, reminder_creation_date) 
VALUES ('meet smriti for lunch', 'location : Chervil Restaurant\ntime : 1:00 PM', 'meet', '2021-02-26');
INSERT INTO notemanagement.reminder (reminder_name, reminder_descr, reminder_type, reminder_creation_date) 
VALUES ('pickup stelli from school', 'location : St. John School\ntime : 3:00 PM', 'meet', '2021-02-26');
```

```
INSERT INTO notemanagement.notecategory (note_id, category_id) 
VALUES ('1', '2');
INSERT INTO notemanagement.notecategory (note_id, category_id) 
VALUES ('2, '2');
INSERT INTO notemanagement.notecategory (note_id, category_id) 
VALUES ('3', '1');
```

```
INSERT INTO notemanagement.notereminder (note_id, reminder_id) 
VALUES ('1', '1');
INSERT INTO notemanagement.notereminder (note_id, reminder_id) 
VALUES ('2', '2');
INSERT INTO notemanagement.notereminder (note_id, reminder_id) 
VALUES ('3', '1');
```

```
INSERT INTO notemanagement.usernote (user_id, note_id) 
VALUES ('1', '1');
INSERT INTO notemanagement.usernote (user_id, note_id) 
VALUES ('2', '1');
INSERT INTO notemanagement.usernote (user_id, note_id) 
VALUES ('3', '2');
```