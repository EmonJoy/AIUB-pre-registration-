📚 Course Search & Routine Builder
A simple PHP + MySQL based web app to search university courses and build a weekly class routine interactively.
🚀 Features
•	🔍 Course Search: Search by code, title
•	📝 Dynamic Results Table: Shows course info with ID, code, section, time, and capacity
•	📅 Routine Builder: Click a row to add the course to a visual routine chart
•	⚡ Clash Detection: Prevents adding overlapping courses
•	🗑 Clear Routine: One-click reset with local storage cleanup
•	💾 Persistent Storage: Selected courses are stored in browser localStorage
•	🎨 UI/UX: Bootstrap 5 styling + custom animations for better experience
🛠️ Tech Stack
•	Frontend: HTML, CSS, JavaScript, Bootstrap 5
•	Backend: PHP (MySQLi)
•	Database: MySQL (offered_courses table)

**YOU can access site from this link --> [https://emon.ct.ws/bigpro.php](https://emon.ct.ws/)**


📂 Project Structure

/project-root
 ├── db.php              # Database connection
 ├── index.php           # Main frontend + search + routine logic
 ├── offered_courses.sql # Sample DB (you need to create this table)
 └── README.md           # Project documentation


📸 Screenshots
- Search Panel
- Course Table
- Weekly Routine Chart
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/f9348217-8295-40e2-98e7-e453fd33d144" />

<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/cbb3fa37-72a6-4fce-b8db-f630b4dc444b" />



🔮 Future Improvements
•	User login & personal routine save in DB
•	Export routine as PDF/Excel
•	Dark mode
