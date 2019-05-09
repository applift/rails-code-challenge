# Applift Rails code challenge
The purpose of the challenge is to get an idea of your development style and skills

## Description
Create RoR application where user can create multiple API endpoints by specifying SQL and returns query results as JSON.
Do not over complicate the implementation. Just make sure you follow all the standards that you’d follow in a real project. Feel free to use any gems thay you want.

Please don't spend more than 3 hours on this task. After that time stop coding and send us the result. We prefer that you will use github or gitlab, and send us the repo.

Mock data you can find in [imports.sql](./imports.sql).


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
John uses UI to create endpoint with name `imports_from_djibouti` and with sql:

```
select * from imports where country = 'Djibouti';
```

John now can use URL `my-app.com/api/imports_from_djibouti` that will return JSON:
```
[
  {
    'id': 8,
    'country': 'Djibouti',
    'payout': 8.15,
    'ip': '255.186.77.245',
    'timezone': 'Africa/Djibouti',
    'version': '6.54'
  }
]
```
---
Good luck! 🤞
