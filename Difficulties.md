Throughout the development of your Wildlife Conservation Web App, you encountered several key challenges. Here’s a breakdown:

1️⃣ Frontend Challenges
✅ Design & Layout Adjustments

You wanted specific hero section designs and grid-based layouts for events and news pages.

You iterated on the CSS multiple times to align the styles with your expectations.

You wanted proper alignment for headers, footers, and buttons.

✅ JavaScript Fetch API Issues

Initially, fetching news and events from the backend didn’t work correctly.

You had to ensure that API calls were structured properly and connected to Flask.

✅ Dynamic Content Updates

Wanted news articles and events to be dynamically displayed from the database instead of hardcoded content.

Ensured that JavaScript functions were correctly rendering fetched data.

2️⃣ Backend Challenges
✅ Database Selection & Transition

Initially considered SQLite but later decided to use MongoDB Atlas for scalability.

Needed to convert relational tables into document-based collections.

✅ Setting Up Flask with MongoDB

Had difficulties in connecting Flask to MongoDB Atlas.

Needed a proper .env file configuration for secure database access.

✅ Admin Authentication (JWT)

Implementing JWT-based authentication for the admin panel took extra consideration.

Needed a way to secure routes so only admins could post/edit/delete news and events.

✅ API Endpoint Debugging

Some routes for adding/editing news and events didn’t function as expected.

Required fixing the POST, PUT, and DELETE methods in Flask.

3️⃣ Full-Stack Integration Challenges
✅ Ensuring Frontend & Backend Communication

Ensuring the frontend JavaScript properly interacted with the Flask backend.

Fixed CORS issues that blocked frontend requests.

✅ Deployment Concerns

Wanted to deploy the backend on Render/Heroku and the frontend on Netlify/GitHub Pages.

Needed proper API URL adjustments for a smooth connection in production.

✅ Refactoring for Simplicity

Initially considered adding donations, but later decided to remove the feature to focus on core functionalities.

Final Thoughts & Next Steps
You’ve now successfully structured your project, solved multiple frontend-backend integration issues, and optimized your MongoDB schema.

Would you like help with final deployment steps or additional features?
