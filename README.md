# 🩸 Blood Bank Management System – Person 1 Frontend

Frontend for the Blood Bank Management System using **HTML, CSS, JavaScript and Bootstrap 5**.

## Features
- Home page
- Login and registration
- Donor dashboard
- Hospital dashboard
- Admin dashboard
- Blood search
- Blood request form
- Responsive Bootstrap UI
- Mock data for frontend demonstration
- Central API helper ready for Spring Boot integration

## Folder Structure
```text
frontend/
├── index.html
├── login.html
├── register.html
├── donor-dashboard.html
├── hospital-dashboard.html
├── admin-dashboard.html
├── blood-search.html
├── blood-request.html
├── css/
│   └── style.css
├── js/
│   ├── app.js
│   ├── login.js
│   ├── register.js
│   ├── blood.js
│   ├── request.js
│   └── admin.js
└── images/
```

## Run
Open `index.html` in a browser, or use VS Code Live Server.

## Backend Integration
Person 2 can change:
```js
const API_BASE_URL = "http://localhost:8080/api";
```
in `js/app.js`.

Expected API examples:
- `POST /api/auth/login`
- `POST /api/auth/register`
- `GET /api/blood-stock`
- `POST /api/blood-requests`
- `GET /api/blood-requests`
- `GET /api/users`

The exact endpoints should be changed to match the Spring Boot backend contract agreed by the team.

## Important
The current login, registration, inventory, dashboards and requests use **demo/mock data**. Do not use this frontend-only login for a real production system. Authentication and authorization must be implemented by Spring Security in the backend.
