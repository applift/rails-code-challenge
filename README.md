# Applift Rails code challenge
The purpose of the challenge is to get an idea of your development style and skills

## Descprition
Create RoR application where user can create multiple API endpoints by specifying SQL and returns query results as JSON.
Do not over complicate the implementation. Just make sure you follow all the standards that you’d follow in a real project. Feel free to use any gems thay you want.

Please spend 3 hours on this task. After that time stop coding ans send us the result. We prefer that you will use github or gitlab, and send us the repo.

Mock data you can find here: `TODO: add mock data`

## Features
As user I want:
- Create/edit/delete endpoint with UI
- When creating I want to define SQL query and endpoint URL
- Create stats page for each endpoint - how many requests were:
  - In total
  - Today
  - In last 6h, 12h, 24h
- Access data from the API endpoint

Other requirements:
- Endpoint queries will be only `select` queries.

## Example:
John uses UI to create endpoint with name `users_from_us` and with sql:

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
