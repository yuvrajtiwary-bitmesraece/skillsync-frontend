# SkillSync Frontend

SkillSync Frontend is a clean, responsive user interface built using vanilla HTML, CSS, and JavaScript that enables seamless interaction with the SkillSync backend API for real-time user registration, authentication, and skill management.

## Features

- Intuitive registration and login forms with form validation
- Seamless integration with backend via RESTful API
- Token-based authentication handling using JavaScript
- Profile retrieval and update functionality
- Add, delete, and view user skills dynamically
- Fetch and display community users and skill statistics
- Responsive and accessible UI design for smooth user experience
- Loading overlay and alert handling for API feedback

## Tech Stack

### Frontend
- **HTML5** – Semantic structure and markup
- **CSS3** – Styling and layout with responsive design
- **Vanilla JavaScript (ES6+)** – DOM manipulation, API integration, and event handling

### Communication
- **Fetch API** – Handles all RESTful requests to the backend
- **JWT Handling** – Uses Bearer token for secure API access

## Installation & Setup

Follow the steps below to run the frontend locally:

1. **Clone the repository**
   ```
   git clone https://github.com/yuvrajtiwary-bitmesraece/skillsync-frontend.git
   cd skillsync-frontend
   ```
   
2. **Open index.html**
   ```
   You can use any live server extension in VS Code or simply open index.html in your browser.
   ```

3. **Connect to Backend**
   ```
   - Ensure the SkillSync backend is running and accessible.
   - Update the backendURL in your JavaScript (if needed) to point to the correct backend deployment.
   ```

You're all set to explore SkillSync frontend locally!

## Folder Structure

Below is the high-level structure of the frontend directory:

```
skillsync-frontend/
├── index.html # Main HTML file
└── README.md # Project documentation
```

## API Integration (Endpoints Used)

The frontend communicates with the SkillSync backend via the following REST API endpoints:

```
| Endpoint                     | Method  | Description                                 |
|------------------------------|---------|---------------------------------------------|
| `/api/auth/register`         | POST    | Register a new user                         |
| `/api/auth/login`            | POST    | User login and token retrieval              |
| `/api/user/profile`          | GET     | Fetch logged-in user’s profile details      |
| `/api/user/profile`          | PUT     | Update logged-in user’s profile information |
| `/api/user/skills`           | GET     | Get logged-in user’s skills                 |
| `/api/user/skills`           | POST    | Add a new skill to user’s profile           |
| `/api/user/skills/:skill`    | DELETE  | Remove a skill from user’s profile          |
| `/api/user/all`              | GET     | Retrieve all users (admin/authorized users) |
| `/api/user/skills/stats`     | GET     | Retrieve aggregated skill statistics        |

- All endpoints requiring user authentication expect a JWT token in the `Authorization` header:  
- `Authorization: Bearer <token>`
```

This setup ensures secure and efficient data exchange between frontend and backend.

## Screenshots

### 1. Welcome Screen  
![Welcome Screen](https://raw.githubusercontent.com/yuvrajtiwary-bitmesraece/skillsync-frontend/main/Welcome%20Screen.png)  

User registration and login forms for seamless onboarding.

### 2. Main Dashboard  
![Main Dashboard](https://raw.githubusercontent.com/yuvrajtiwary-bitmesraece/skillsync-frontend/main/Main%20Dashboard.png)  

Displays user profile, skill management, and community sections.



## Thank You

Grateful for your time and attention — it truly means a lot!


