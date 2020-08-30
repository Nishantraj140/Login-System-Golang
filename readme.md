### Golang MySQL Login-System 

### How To Run 

Create a new database named go_db with a users table 

```sql
CREATE TABLE users(
    id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    email VARCHAR(120),
    password VARCHAR(120),
    full_name VARCHAR(120),
    contact_email VARCHAR(200),
    address VARCHAR(255),
    phone VARCHAR(45)
);
```


Inside of **main.go** line **26** replace password with your own credentials

```go
db, err = sql.Open("mysql", "<root>:<password>@/go_db")
// Replace with 
db, err = sql.Open("mysql", "myUsername:myPassword@/myDatabase")
```
