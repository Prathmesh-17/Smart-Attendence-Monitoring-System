Introduction : A biometric attendance system that uses a fingerprint sensor to accurately identify users and automatically record attendance in real time. Designed to eliminate proxy attendance and bring automation to academic and workplace environments.

Components Used : 
Hardware 
Fingerprint sensor: scans fingerprint, creates template, matches against stored templates.
Microcontroller (Arduino Uno) : controls sensor, triggers enrollment/authentication, timestamps events and writes attendance records.
LCD : shows prompts like “Present”.
LED: audible / visual confirmation for success/fail.
Storage (SD card): persistent storage of attendance logs for reporting.
Power Supply (5v)

Softwere : 
Arduino Ide

Working 
When the system is powered on, the Arduino initializes the fingerprint sensor, RTC, SD card, and LCD. When a user places their finger on the sensor, it scans and compares the fingerprint with the stored templates. If a match is found, the Arduino fetches the current date and time from the RTC and saves the attendance record to the SD card in CSV format. The LCD display shows messages like “Match Found” and “Attendance Marked.” If no match is found, the LCD shows an error message.


