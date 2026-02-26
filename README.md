A lightweight, high-performance web application designed to streamline student complaint management. This system provides a seamless interface for students to voice concerns and a robust dashboard for administrators to track, filter, and resolve issues with complete transparency.

🚀 Key Features
Student Portal
Secure Authentication: Dual-role login with CAPTCHA validation to prevent automated spam.

Instant Submission: Lodge complaints across multiple categories (Hostel, Faculty, Infrastructure).

Automated Tracking: Every complaint generates a Unique Ticket ID for real-time status monitoring (Pending vs. Resolved).

Admin Dashboard
Real-time Analytics: Visual counters for total, pending, and resolved complaints.

Privacy-First Interface: - Identity Masking: Student names are displayed as "Anonymous" in the dashboard.

Data Obfuscation: Registration numbers are hidden using asterisks to ensure unbiased grievance handling.

Advanced Management: Searchable tables with filters for category and status.

Data Portability: Integrated CSV Export for offline reporting and administrative meetings.

🛠️ Technical Stack
This project follows a "Lean Web" philosophy, focusing on speed and native browser capabilities without heavy external dependencies.

Frontend: HTML5 & Tailwind CSS (Utility-first styling for a modern, responsive UI).

Logic: Vanilla JavaScript (ES6+) for high performance and native DOM manipulation.

Data Persistence: Web Storage API (localStorage) — used to simulate a backend environment by storing data directly in the browser.

Typography & Icons: Inter Google Font & custom SVG iconography.

🏗️ Architecture & Security
The system is designed to be a functional Minimum Viable Product (MVP) with a focus on data integrity:

Serialization: JavaScript objects are converted to JSON strings using JSON.stringify() for storage and reconstructed using JSON.parse() for UI rendering.

Auth Guards: Implements a session-based authentication flag (cmsAdminLoggedIn) to prevent unauthorized access to the admin panel via URL manipulation.

Frontend Security: Uses JavaScript logic to ensure only the student who created a complaint can view their specific history.

🗺️ Roadmap (Future Enhancements)
While the current version is fully functional as a client-side tool, the future roadmap includes:

[ ] Cloud Integration: Transitioning to Node.js/Firebase for global data persistence across different devices.

[ ] Automated Alerts: Implementing Email Notifications to update students when a ticket status changes.

[ ] Role-Based Access: Adding different permissions for Department Heads vs. Campus Maintenance.

[ ] Advanced Security: Integrating Password Hashing (Bcrypt) and JWT for enterprise-grade security.
