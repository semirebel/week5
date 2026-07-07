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
