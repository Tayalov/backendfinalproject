Medline  
SE-2434
Talgatova Ayaulym
Final Project Report – MedLine App
1. Project Overview 

The MedLine application is a full-stack web application designed to manage medical data, including doctors, patients, and medicines. Users can view medicine ratings, see doctor prescriptions, and manage their personal profiles. The application implements authentication, role-based access control (RBAC), and CRUD operations for all main entities.

2. System Architecture 

The project uses a Node.js/Express backend with MongoDB for database management. The frontend is built using HTML, CSS, and JavaScript with dynamic data fetching via API calls. The architecture follows the MVC pattern (Model-View-Controller) to separate concerns.
•	Backend: Node.js, Express, JWT authentication, Mongoose ODM
•	Frontend: HTML, CSS, JavaScript, responsive design
•	Database: MongoDB with collections for Users, Patients, Doctors, Medicines, Prescriptions
•	Middleware: Authentication and role-based access control
<img width="394" height="1445" alt="image" src="https://github.com/user-attachments/assets/dd8eb74f-e17b-49ef-a558-c94772a1ba92" />

 <img width="380" height="1389" alt="image" src="https://github.com/user-attachments/assets/4afaed42-ec23-4f97-ac01-fdfee3e2a1fc" />

 
3. Features 
English:
1.	User Authentication: Registration, login, and JWT-based session management
2.	Role-Based Access Control (RBAC):
o	Admins can add, edit, and delete medicines and doctor data
o	Patients can view medicines and their personal prescriptions
3.	CRUD Operations:
o	Medicines: Create, Read, Update, Delete
o	Doctors: Create, Read, Update, Delete
o	Prescriptions: Read only for patients, full CRUD for doctors/admins
4.	Responsive Frontend: Compatible with desktop and mobile screens
5.	Dynamic UI: Data updates without page reload using JavaScript fetch API
 <img width="974" height="262" alt="image" src="https://github.com/user-attachments/assets/fad772cd-89cd-4485-afd5-065994830cd7" />

 <img width="974" height="901" alt="image" src="https://github.com/user-attachments/assets/fe7370d9-c469-4e1c-980c-7cc6d7fabe58" />

4. Implementation 
English:
•	Backend: Node.js with Express; routes separated by entity; controllers implement CRUD logic; JWT authentication and RBAC middleware protect sensitive actions.
•	Database: MongoDB collections: Users, Doctors, Patients, Medicines, Prescriptions. Relationships are maintained via ObjectId references.
•	Frontend: HTML/CSS for layout; JavaScript fetch API connects to backend; forms handle login, registration, and CRUD actions; dynamic updates reflect backend data in real time.
Medicines:
•	 <img width="974" height="688" alt="image" src="https://github.com/user-attachments/assets/9ab2afd4-73c2-48c2-9fc5-25c2443aa464" />

            Prescriptions:
•	 <img width="974" height="639" alt="image" src="https://github.com/user-attachments/assets/6daa8996-37c2-4291-aa2f-c535b636895c" />


Revies:
 <img width="974" height="738" alt="image" src="https://github.com/user-attachments/assets/78dc06cb-4b56-4ad3-99de-28fa95a4bc20" />

Users:
 <img width="974" height="732" alt="image" src="https://github.com/user-attachments/assets/f3303451-4c6a-4d65-b946-fab30a525c95" />

5. Deployment 
English:
•	Backend & Frontend: Deployed together on Render using Node.js deployment.
•	Environment Variables: .env file stores MONGODB_URI and JWT_SECRET.
•	 URL: https://github.com/Tayalov/backendfinalproject.git
•	Postman Collection: Final tests cover all endpoints, including authentication, CRUD, and RBAC actions.
 <img width="974" height="384" alt="image" src="https://github.com/user-attachments/assets/30632386-ab26-4597-83af-78f167ea8eec" />

6. Challenges and Solutions 
English:
•	Challenge: Ensuring RBAC security while keeping dynamic frontend functional
•	Solution: Created middleware functions and tested all endpoints with different roles.
•	Challenge: Deploying MongoDB connection securely
•	Solution: Used environment variables and Render secrets to store sensitive information
•	7. Conclusion 

The MedLine project demonstrates full-stack integration, secure authentication, role-based access, and a responsive, dynamic frontend. It is deployed online and ready for real-world use.



