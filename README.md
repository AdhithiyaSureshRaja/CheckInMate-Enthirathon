# RFID-Attendance-Tracker-Enthirathon
🔹 Project Overview
  This project is designed to automate attendance and track student performance in educational institutions using RFID technology.
  Students scan their RFID cards upon entering class, and their attendance is updated in real time in a Google Sheet.
  Additionally, the system integrates with AppSheet to enable convenient, real-time access to attendance data by both professors and students.


🔹 Features
  ✅ Automated Attendance:
  Using RFID tags for convenient and accurate attendance marking.
  
  ✅ Real-Time Data Update:
  Student data is updated directly to a Google Sheet in real time.
  
  ✅ App Integration (CheckInMate):
  Provides a convenient platform for professors to view attendance, grades, and student achievements, while allowing students to track their own progress.
  
  ✅ Two-step Verification (Optionally Enabled):
  Verifies attendance by matching RFID scan with a secondary login, adding additional authenticity.
  
  ✅ Face Detection (Optionally Enabled with OpenCV):
  Provides additional validation by matching the face with the RFID tag’s owner.


🔹 Hardware
  ESP8266 (with built-in WiFi)
  
  MFRC522 RFID Reader/Writer Module
  
  LCD Display (I2C) 16x2
  
  LED Indicator


🔹 Software
  Arduino IDE (C++ code)
  
  Google Apps Script (for Google Sheets API)
  
  AppSheet (for UI)

🔹 How It Works
  Each student is issued an RFID tag with a unique identifier.
  
  The student scans their RFID tag upon entering the classroom.
  
  The ESP8266 reads the tag’s data and sends it to Google Sheets in real time.
  
  The Google Apps Script parses the data and saves it in the appropriate sheet.
  
  The AppSheet application(CheckInMate) displays updated attendance and related information to professors and students.

🔹 File Structure

 ├── Arduino/
    └ student_attendance.ino
 └─ GoogleAppsScript/
    └ script.gs
 └─ RFID/
    └ rfid_data.ino
 └─ docs/
    └ circuit_diagram.png

🔹 Installation
  Set up your ESP8266 and connect to your WiFi.
  
  Write the code to your ESP8266 with Arduino IDE.
  
  Create a Google Apps Script to connect to your Google Sheet.
  
  Deploy Google Apps Script and enable its API.
  
  Create AppSheet application from your Google Sheet.

🔹 How to Use
  Staff: view real-time attendance, grades, and achievements in AppSheet.
  
  Students: track their own attendance and progress through AppSheet.
  
  Optionally: enable two-step verification or face-detect for additional authenticity.

🔹 Security
  Each tag contains a unique identifier.
  
  Communication to Google Sheets is over SSL/TLS.
  
  User authentication controls enable authorization and data protection.

  Two-Factor Authentication : 
  
  ![image](https://github.com/user-attachments/assets/28088e0e-55da-4fe9-a4aa-0bc8b56245e7)

  Proximity Sensor:

  ![image](https://github.com/user-attachments/assets/4b874b94-ced1-4c9e-bf81-84c5a295441a)


🔹 Future Improvement Ideas
  Implement SMS notifications for low attendance.
  
  Integrate with OpenCV face recognition for additional robustness.

  ![image](https://github.com/user-attachments/assets/88908d02-3a9f-4c58-b0ec-ef293717bbc6)

  
  Provide analytic charts for student attendance over time.

🔹Final Product Overview & Presentation :

  ![WhatsApp Image 2024-10-03 at 20 35 56_848d2cba](https://github.com/user-attachments/assets/f196649a-a4f5-44d6-9938-edb1a48ae61d)
  
  ![image](https://github.com/user-attachments/assets/14d54785-e03a-41a4-813d-b4aed7490b60)



  

