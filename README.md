# Week5

Task 2:
```sql
CREATE DATABASE website;

CREATE TABLE member (
    id INT UNSIGNED NOT NULL AUTO_INCREMENT,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL,
    password VARCHAR(255) NOT NULL,
    follower_count INT UNSIGNED NOT NULL DEFAULT 0,
    time DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP,

    PRIMARY KEY (id)
);
```
<img width="1200" height="799" alt="image" src="https://github.com/user-attachments/assets/6b8afa67-b7db-4052-a6ce-78e9f77772eb" />


Task 3:
```sql
INSERT INTO member (name, email, password) VALUES ('test', 'test@test.com', 'test');
INSERT INTO member (name, email, password, follower_count) VALUES ('Jordan', 'jordanfisher@test.com', 'j0000', '384');
INSERT INTO member (name, email, password, follower_count) VALUES
('Talia', 'taliaryder@test.com', 't0000', '40');
INSERT INTO member (name, email, password, follower_count) VALUES
('Sam', 'samclaflin@test.com', 's0000', '389');
INSERT INTO member (name, email, password, follower_count) VALUES
('Lily', 'lilycollins@test.com', 'l0000', '2848');
```
<img width="1684" height="541" alt="image" src="https://github.com/user-attachments/assets/d462eb82-923a-40d7-b742-74e15e28326f" />

```sql
SELECT * FROM member;
SELECT * FROM member ORDER BY time DESC;
```
<img width="1150" height="704" alt="image" src="https://github.com/user-attachments/assets/46596e9d-cdc4-4d5e-865f-79db6e9e0901" />

```sql
SELECT * FROM member ORDER BY time DESC LIMIT 1, 3;
SELECT * FROM member WHERE email = 'test@test.com';
SELECT * FROM member WHERE name LIKE '%es%';
```
<img width="1386" height="784" alt="image" src="https://github.com/user-attachments/assets/0f209ecf-e822-4511-8c77-42f57974473f" />

```sql
SELECT * FROM member WHERE email = 'test@test.com' AND password = 'test';
UPDATE member SET name = 'test2' WHERE email = 'test@test.com';
```
<img width="1198" height="457" alt="image" src="https://github.com/user-attachments/assets/80c43570-a306-43bc-a71c-028b96ae983f" />
