📸 README: Instagram Clone

Project Overview:
This porject is a basic backend and frontend system designed to mimic core functionalities of Instagram.
It serves as a demonstration of fundamental Full-Stack development skills, including use3r authentication ,
complex database relationship (following/followers),content creation, and dynamic feed generation.

✨ Features Implemented:
The application provides the following core features:

Backend Requirement: 

1. User Authentication 
● User signup 
● User login 
● Password hashing 
● Return a token/session for authenticated routes

2. Follow System 
● A user should be able to follow another user 
● A user should be able to unfollow 
● You should maintain proper relationships

3. Post Creation 
● Authenticated users can create posts 
● A post should have: 
○ Image URL (string) 
○ Caption (string)

4. Likes 
● Users should be able to like a post 
● Users should be able to unlike a post

5. Comments 
● Users should be able to comment on posts 
● Comments should show who commented and what they wrote

6. Feed 
● Create an API to fetch a “feed” of posts 
● Feed must show posts created by the users whom the logged-in user follows

Frontend Requirements: 
You may use React, Next.js, Angular, or Vue (React recommended and Nextjs). 

Screens to build: 
Screen                    Features 
● Login & Signup          Store token securely, redirect on login
● Home Feed               List of posts with image, caption, likes, and comments 
● Create Post             Form to add new post (image URL + caption) 
● Profile Page            User posts, follower/following count, Follow/Unfollow button
● Post Detail             Full view, interactive like/comment UI

Frontend Features: 
● Use Fetch API or Axios for API calls 
● Display data dynamically 
● Update UI without page refresh (state management) 
● Basic clean responsive design 

⚙️ Running the Application: 
Follow these steps precisely to get both the backend API and the frontend client running 
on your local machine.

Prerequisites Check
Before starting, ensure you have completed the following:

1.The project repository is cloned.
2.Database (e.g., MongoDB, PostgreSQL) is installed and running.
3.All dependencies have been installed in both the backend and frontend folders using npm install.
4.The .env file in the backend directory is correctly configured with your DB_URI and JWT_SECRET.

Step 1: Start the Backend Server:
The backend provides the API endpoints for user authentication, posts, following, and the feed.

i.Navigate to the backend directory:
cd backend

ii.Start the server:
# This command starts your Node.js server (e.g., Express)
npm start 
# OR, if you use nodemon for live reload during development:
# npm run dev

Output: The console should show a message indicating the server is running.
Server running on port 5000
MongoDB Connected

Step 2: Start the Frontend Application:
The frontend will provide the user interface for the Login, Home Feed, Profile, and Post Creation screens.

i.Navigate to the frontend directory:
# Go back to the root and then into the frontend (or just to the root if your frontend is there)
cd ..
cd frontend

ii.Launch the development server:
# This command starts your React/Vite development server
npm run dev
Output: The console will provide a local and network URL
Local:   http://localhost:5173/
Access: Open the provided Local URL in your web browser.

Step 3: Test Functionality:

i.User Flow: Begin by testing the Signup route and then Login.

ii.Feed Test: Create a few users, follow one of them , and ensure the personalized Home Feed displays posts only
from the followed user.

Summary:

Deliverable               Status & Brief                                                          Focus Area  
1. Database Design        Ready for Implementation. You need to translate the relational          Backend Setup                        
                          database system (e.g., MongoDB, PostgreSQL). This is the foundation
                          for your backend logic.
2. API Design             Ready for Implementation. This involves building the specific           Backend Logic
                          endpoints (e.g., POST /api/auth/login, POST /api/users/:id/follow,
                          GET /api/posts/feed) that will be handled by your Node.js server.
3. Node.js Project        In Progress / Missing. This is your primary task. The files you         Backend Development
    with working          provided are for the Frontend (React/Vite). You still need to create
    endpoints             the separate Backend project (likely a folder named backend/) using
                         Node.js and a framework like Express.js to implement the API design and
                         connect to the database.
4. Postman Collection    Missing. Once your Node.js endpoints are built, you must create a        Testing & Submission
                         Postman collection containing all the API routes (Login, Signup, Create
                         Post, Follow, etc.) and save the collection file in your repository. This
                         proves the endpoints work.
