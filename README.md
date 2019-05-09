# Applift Rails code challenge
The purpose of the challenge is to get an idea of your development style and skills. The way you structure code, tests, etc.

## Desciprition
Create RoR application where user can create multiple API endpoints by specifying SQL and returns query results as JSON.
Do not over complicate the implementation. Just make sure you follow all the standards that you’d follow in a real project.
Feel free to use

Mock data you can find here: `TODO: add mock data`

## Features
As user I want:
- Create/edit/delete endpoint
- When creating I want to define SQL query and endpoint URL
- See endpoint stats - how many requests were:
  - In total
  - Today
  - In last 6h, 12h, 24h
- Access data from the API endpoint

## Example:
John creates endpoint called `users_from_us`, with sql:

```
select * from users where country = 'us';
```

John now can use URL `my-app.com/api/users_from_us` that will return JSON:
```
[
  { name: "John", last_name: "Doe"}
]
```
---
Good luck! 🤞
