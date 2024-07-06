# PostgreSQL

# Init and Config
1. Start and Stop PostgreSQL:
```
brew services start postgresql
brew services stop postgresql
brew services restart postgresql
```

2. The default PostgreSQL user (usually postgres)
```
psql -U postgres
```
Password: 1234

3. Access PostgreSQL:
```
psql postgres
```

4. Create a new PostgreSQL user from any user:
```
CREATE USER new_user WITH PASSWORD 'new_password';
```

5. Grant necessary privileges to the new user (optional, depending on your requirements):
```
ALTER USER new_user WITH SUPERUSER;
```

6. Access PostgreSQL with the new password:
```
psql -U new_user
```
7. List all users (roles):
```
\du 
