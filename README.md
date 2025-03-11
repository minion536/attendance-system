# Real-Time Face Recognition-Based Attendance System

## Overview
The **Real-Time Face Recognition-Based Attendance System** is an AI-powered solution designed to automate attendance tracking using facial recognition. This system ensures accurate and efficient attendance management by leveraging computer vision and a MySQL database.

![take attendace page](https://github.com/user-attachments/assets/d24ba5a0-54b0-477d-8e3f-cf73f97049bc)

![view attendance page](https://github.com/user-attachments/assets/af7a4e9c-2f8a-4961-91db-b10fd341a2ce)

## Features
- **Face Recognition:** Uses AI-based facial recognition for attendance marking.
- **MySQL Database Integration:** Stores user details and attendance records.
- **Automated Attendance Marking:** Detects and records attendance in real-time.
- **Admin Dashboard:** Provides an interface for managing students and attendance records.
- **Excel Export:** Generates attendance reports in Excel format for easy analysis.
- **Hardware Compatibility:** Deployable on high-performance **GeForce RTX 5070** setups.

## Technologies Used
- **Backend:** Node.js with Express.js
- **Database:** MySQL with `userDetails` and `attendance` tables
- **Frontend:** Streamlit (for interface, if applicable)
- **AI/ML:** OpenCV, Deep Learning (face recognition model)
- **Deployment:** Docker (for PostgreSQL alternative setups)

## Database Schema
### `userDetails` Table
| Column Name | Data Type | Description |
|------------|----------|-------------|
| id | INT (Primary Key) | Unique ID for each user |
| name | VARCHAR | Name of the individual |
| image | BLOB | Stored image data for facial recognition |

### `attendance` Table
| Column Name | Data Type | Description |
|------------|----------|-------------|
| id | INT (Primary Key) | Unique attendance record ID |
| user_id | INT (Foreign Key) | Reference to `userDetails.id` |
| timestamp | TIMESTAMP | Time when attendance was recorded |

## Installation and Setup
### Prerequisites
- **Python** (for AI model and Streamlit, if used)
- **Node.js** (for backend APIs)
- **MySQL Server** (for database management)
- **Docker** (for PostgreSQL alternative, if applicable)

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/attendance_system.git
   cd attendance_system
   ```
2. Install backend dependencies:
   ```sh
   cd backend
   npm install
   ```
3. Set up MySQL database:
   - Create `userDetails` and `attendance` tables.
   - Use stored procedures and triggers for automation.
4. Start the backend server:
   ```sh
   node server.js
   ```
5. (Optional) Run the AI model for facial recognition:
   ```sh
   python face_recognition.py
   ```
6. (Optional) Start the Streamlit frontend:
   ```sh
   streamlit run app.py
   ```

## Usage
- **Admin:** Adds users by uploading images and assigning IDs.
- **Users:** Stand in front of the camera for real-time recognition.
- **Attendance Logs:** View and export attendance records.

## Future Enhancements
- **Raspberry Pi Deployment** for low-cost, portable solutions.
- **Mobile App Integration** for real-time attendance updates.
- **Cloud Storage Support** to save images securely.
- **Enhanced AI Model** with deep learning for improved accuracy.

## License
This project is licensed under the MIT License.

## Author
Developed by **ANWAR SHAIK**, a full-stack developer and AI/ML researcher.

---
*For any queries or contributions, feel free to reach out!*

