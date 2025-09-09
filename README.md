📚 Course Search & Routine Builder
A simple PHP + MySQL based web app to search university courses and build a weekly class routine interactively.
🚀 Features
•	🔍 Course Search: Search by code, title, or faculty
•	📝 Dynamic Results Table: Shows course info with ID, code, section, faculty, time, and capacity
•	📅 Routine Builder: Click a row to add the course to a visual routine chart
•	⚡ Clash Detection: Prevents adding overlapping courses
•	🗑 Clear Routine: One-click reset with local storage cleanup
•	💾 Persistent Storage: Selected courses are stored in browser localStorage
•	🎨 UI/UX: Bootstrap 5 styling + custom animations for better experience
🛠️ Tech Stack
•	Frontend: HTML, CSS, JavaScript, Bootstrap 5
•	Backend: PHP (MySQLi)
•	Database: MySQL (offered_courses table)
📂 Project Structure

/project-root
 ├── db.php              # Database connection
 ├── index.php           # Main frontend + search + routine logic
 ├── offered_courses.sql # Sample DB (you need to create this table)
 └── README.md           # Project documentation

🗄️ Database Setup
1.	Create a database named bigpro.
2.	Create a table offered_courses with columns like:

CREATE TABLE offered_courses (
    class_id INT AUTO_INCREMENT PRIMARY KEY,
    course_code VARCHAR(20),
    course_title VARCHAR(100),
    section VARCHAR(10),
    faculty VARCHAR(100),
    day VARCHAR(20),
    start_time VARCHAR(20),
    end_time VARCHAR(20),
    capacity INT,
    count INT
);

Insert some sample data:

INSERT INTO offered_courses (course_code, course_title, section, faculty, day, start_time, end_time, capacity, count)
VALUES
('CSE101', 'Intro to Programming', 'A', 'Dr. Rahman', 'Sunday', '10:00 AM', '11:30 AM', 40, 35),
('MAT201', 'Discrete Math', 'B', 'Prof. Karim', 'Tuesday', '2:00 PM', '3:30 PM', 50, 42);

▶️ How to Run
1. Clone or download the project:
git clone https://github.com/your-username/course-routine.git
cd course-routine
2. Place files in htdocs (if using XAMPP).
3. Import offered_courses.sql into MySQL.
4. Start Apache & MySQL.
5. Open in browser: http://localhost/course-routine
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
